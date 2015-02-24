{{:WPD:Infrastructure/architecture}}
= Reports to review status =

From the  [[WPD:Infrastructure/architecture/The_salt_master|The Salt Master]] we can get various system health status. This document describes how to access them.

__TOC__

= Reports =

== How many emails has been sent ==

We have  [http://mailgraph.schweikert.ch/ ''Mailgraph''] installed on all ''mail'' VMs. With it, we can visualize how many emails are being sent to our mail server. It should display the number of refusals (e.g. somebody outside our network trying to use us) over time.

From the browser, through [[#Read reports from a VM through private network]].

  http://mail/cgi-bin/mailgraph.cgi

Should look like this:

[[File:20150106_mailgraph_day.png]]
[[File:20150104_mailgraph_day.png]]

'''Note''' that this screenshot was made to illustrate a crisis we’ve had but you can see notes that should illustrate what we can get from the reports.

== Getting to know the status of a php5-fpm backend ==

You can make a basic ''GET /fcgi-status'' to any VMs that has '''php5-fpm''' running. (@@TODO make a role to get all of them and remove the need to guess)

There are a few variants we can get data;

* Simple report

  curl piwik/fcgi-status

* A more detailed version

  curl piwik/fcgi-status?full

[[File:nginx_fastcgi_status_full.png]]
[[File:nginx_fastcgi_status.png]]

'''Note''' that in this example I used an SSH tunnel ''-L 8080:piwik:80'', but it could have been done through [[#Read reports from a VM through private network]].

== Getting to know the status of an NGINX web server ==

* From the local network

  curl piwik/nginx-status
  Active connections: 1
  server accepts handled requests
   3031 3031 3024
  Reading: 0 Writing: 1 Waiting: 0

* From salt

  salt piwik nginx.status
  piwik:
    ----------
    accepted:
        3030
    active connections:
        1
    handled:
        3030
    reading:
        0
    requests:
        3023
    waiting:
        0
    writing:
        1
  

== Getting to know the status of an Apache2 web server ==

* From salt

  salt app\* apache.server_status
  app3:
    ----------
    BusyWorkers:
        3
    BytesPerReq:
        865.907
    BytesPerSec:
        3152.89
    CPULoad:
        0.300867
    IdleWorkers:
        16
    ReqPerSec:
        3.64114
    Scoreboard:
        ----------
        .:
            45
        C:
            2
        D:
            0
        G:
            0
        I:
            0
        K:
            0
        L:
            0
        R:
            0
        S:
            0
        W:
            1
        _:
            16
    Total Accesses:
        40748
    Total kBytes:
        34457
    Uptime:
        11191

== MySQL/MariaDB ==

We can check what’s the state of the MySQL server by issuing the following commands. They are available through [http://docs.saltstack.com/en/latest/ref/modules/all/salt.modules.mysql.html#salt.modules.mysql.get_slave_status ''Salt Stack'' '''mysql''' module]

=== Get replication status ===

  salt db2 mysql.get_slave_status
  db2:
    ----------
    Connect_Retry:
        10
    Master_Host:
        masterdb.local.wpdn
    Master_SSL_Allowed:
        Yes
    Master_SSL_CA_File:
        /etc/mysql/ca-cert.pem
    Master_SSL_Cert:
        /etc/mysql/client-cert.pem
    Master_SSL_Crl:
        /etc/mysql/ca-cert.pem
    Master_SSL_Key:
        /etc/mysql/client-key.pem
  // ... truncated  
 
=== Get replication master status ===

  salt -G 'roles:masterdb' mysql.get_master_status
  db1-masterdb:
    ----------
    File:
        mariadbrepl-bin.000093
    Position:
        32058870
  // ... truncated

=== Get process list ===

  salt -G 'roles:db' mysql.processlist
  db2:
    |_
      ----------
      Command:
          Connect
      Id:
          3
      Info:
          None
      Progress:
          0.0
      State:
          Slave has read all relay log; waiting for the slave I/O thread to update it
      Time:
          1
      User:
          system user
      db:
          None

=== Misc. reports available on MySQL servers through Salt stack  ===

Here are a few possibly useful commands to pick from;

'''Note''' its even possible to work on grants/privileges, add/delete databases. Note that if you do so, you MUST make sure that you do it ONLY on the salt master. To learn more, refer to [http://docs.saltstack.com/en/latest/ref/modules/all/salt.modules.mysql.html#salt.modules.mysql.get_slave_status ''Salt Stack'' documentation at '''mysql''' module].

  salt db2 mysql.get_slave_status
  salt -G 'roles:masterdb' mysql.get_master_status
  salt -G 'roles:db' mysql.status


== MediaWiki ==

Some reports can be gathered from the MediaWiki API. Here’s a list of a few useful ones. If you want to change the way they are displayed, you can change the ''&format='' URL fragment (ref: [https://www.mediawiki.org/wiki/API:Main_page#The_format ''MediaWiki.org'' documentation].

=== Misc. reports ===

* [https://docs.webplatform.org/w/api.php?format=jsonfm&action=query&prop=contributors&continue=&titles=css/properties/border Contributors on '''css/properties/border''' page (through the API)]
* [https://docs.webplatform.org/wiki/Special:Contributions/Renoirb Contributions made by a specific user]
* [https://docs.webplatform.org/w/api.php?format=jsonfm&action=query&list=users&ususers=Renoirb&usprop=blockinfo|groups|editcount|emailable More details about a user (through the API)]

=== User creation log ===

As long as we don’t have a separate accounts system in place for every components, including our wiki, we need to review in each web application the new accounts that are being created. If we have too many accounts created, it means that we might be under spambot attacks.

* [https://docs.webplatform.org/w/api.php?format=jsonfm&action=query&list=logevents&letype=newusers&lelimit=50&leprop=user|timestamp list new users (through the API)]

[[File:20150106-account-creation-log-api.png]]

=== What’s the IP address of a given user? ===

In case of need to review how our infrastructure is being abused, we can get to know the IP address of visitors so that we can effectively ban them.

To do so, we are using the [https://www.mediawiki.org/wiki/Extension:CheckUser ''MediaWiki CheckUser'' Extension]. Only users of the wiki with sysop privileges can review this information.

[[File:20150108-visualizing-visitor-IP-vs-users.png]]

== Using Monit ==

Monit is a software that you can configure to check if a service is accessible or running and how it can make sure its up automatically for you.

'''More about Monit in [[WPD:Infrastructure/Monitoring/Monit]]'''

=== From the salt master ===

We can get '''monit''' reports '''from the salt master''' like this

  salt -G 'roles:app' monit.summary
  app2-jobrunner:
    ----------
    Process:
        ----------
        apache2:
            Running
        nutcracker:
            Running
        openssh-server:
            Running
        salt-minion:
            Running
    System:
        ----------
        app2-jobrunner.production.wpdn:
            Running
  app1:
    ----------
    Process:
        ----------
        apache2:
            Running
        nutcracker:
            Running
        openssh-server:
            Running
        salt-minion:
            Running
    System:
        ----------
        app1.production.wpdn:
            Running

Or from the same VM:

  sudo salt-call monit.summary
  [INFO    ] Executing command 'monit summary' in directory '/root'
  local:
    ----------
    Process:
        ----------
        exim4:
            Running
        gdnsd:
            Running
        openssh-server:
            Running
        salt-master:
            Running
        salt-minion:
            Running
        syslog-ng:
            Running
    System:
        ----------
        salt.production.wpdn:
            Running

=== From the web frontend ===

To do this, you need to create a SOCKS proxy like its described in [[#Read reports from a VM through private network]]

Once connected through ssh with the proxy described, you can connect like this:

  http://monit:p4ssword@sessions1:2812/

Which should look like this;

[[File:20150224-monit-status-preview.png]]

==== Monit password ====

The password is not "p4ssword", you’ll have to look at '''/srv/private/pillar/accounts/''' file yourself at '''accounts:monit:admin_password''' or in the VM itself at '''/etc/monit/conf.d/defaults.conf'''.

An alternate way to get to know the password is to use salt like this:

  salt-call pillar.get accounts:monit:admin_password
  local:
    p4ssword

== Read reports from a VM through private network ==

To work on a cluster on a given level, you can use the salt master as a SOCKS proxy to view privileged reports such as service health and usage reports.  

To view the internal only reports, configure one of your web browser to use your local computer as a proxy through the SSH tunnel we will create.

  ssh salt.webplatform.org -C -D 1080

=== Setting automatically a SOCKS proxy in your SSH configuration ===

Alternately, you can add to your '''~/.ssh/config''' file the following line within the appropriate '''Host''' block.

 ### WPD Production
 Host production.wpdn
   Hostname salt.webplatform.org
   ProxyCommand none
   DynamicForward 1080
 Host *.production.wpdn
   ProxyCommand ssh -e @ -o StrictHostKeyChecking=no -a -W %h:%p production.wpdn

'''Note''' this block is an example of what you can use to have a '''DynamicForward''' automatically installed. 

'''IMPORTANT''' Make sure you always use the connection block that the salt master provides you at connection time as this example here might become outdated.


=== Configuring a web browser to use the proxy ===

Once connected, you have to configure a web browser to use your new '''DynamicForward''' SOCKS proxy. 

In modern Firefox version, you can do that by going into '''Preferences''', '''Advanced''', '''Network''' tab, then '''Connection''' button. You’ll see a window similar to below. Adjust accordingly.

[[File:201502-Firefox-Network-settings.png]]
 
To learn how to configure your web browser to use SSH as a SOCKS proxy, you can view the [https://help.ubuntu.com/community/SSH/OpenSSH/PortForwarding#Dynamic_Port_Forwarding SSH Port forwarding help pages on '''help.ubuntu.com''']