= Hardware and software requirements =

Summarizing server requirements described in length in [[WPD:Infrastructure/analysis/2013-Usage and future state]].

== Summary ==

We are using OpenStack hosted Virtual Machines (VM) as our main computing environment. Our VMs are configured using [http://saltstack.com Salt Stack] to manage instance states and various aspects of OpenStack. Salt is similar to Puppet by managing machine state, but it also enables remote execution and can communicate with OpenStack services.

We require many servers to host our services (memcache, MySQL, NGINX, Varnish, Apache, etc). HTTP requests to these servers are managed by our caching layer, which is provided by [http://fastly.com Fastly]; this provides a caching and CDN service and improves site performance. In the future, we plan to optimize the infrastructure, and implement ''continuous deployment''.

In terms of hosting and server infrastructure, we want to have more than one hosting provider, to enable redundancy and multiple site replication, and to showcase the power of OpenStack. In the short term, we need only a single major host.

== Requirements ==

=== General ===
* Open Stack service environment
* Access to Nova API
* Block storage (Cinder or similar, not in use but planned)
* Open to other managed PaaS service, if available. (e.g. managed ''MySQL'' or ''Memcached'' server)

=== Production environment ===
These are our minimum requirements for the live site:

* 31 vCPU, 102 Gb vRAM, flavors:
** 8x 2 vCPU, 8Gb vRAM (MediaWiki server, slave DB server)
** 1x 4 vCPU, 16Gb vRAM (DB)
** 4x 2 vCPU, 4Gb vRAM
** 3x 1 vCPU, 2Gb vRAM
* 11 IPv4 Public IP addresses

=== Staging and testing environments ===
In addition to the production environment, we want to have a testing and staging deployment running full time.

These environments have the same requirements as the production environment,  deployed in a separate network, but do not need guaranteed uptime.

== Our Infrastructure ==
Every machine is managed by a set of states and pillars and admins manages the complete infrastructure through the Salt master.

This is the current breakdown of machines per service type. Our plan is to eventually slim down the quantity of machines and merge some services together.

=== Distribution by type === 

==== Infrastructure servers ====
* Salt master (1 VM, Public IP)
* NOC nodes (2 VMs, 1 Public IP)
* Memcache (2 VMs)
* MySQL (2 VMs)
* Storage (2 VMs)
* Backup (1 VM)

==== Frontend servers ====
Web server hosting web application, most of them are behind [http://fastly.com Fastly].

* Analytics (2 VMs, Public IP, ''not behind'' Fastly)
* Blog (1 VM, Public IP, Apache)
* App server (5 VMs, Public IP, Apache)
* Project management web app (1 VM, Public IP, Apache)

== Changes ==

=== Current migration ===
What we would appreciate to have in a new environment.

* Storage facility/mount-points 
** Note: We are currently using a set of VMs with Gluster FS
* Routing to allow downloading from the Internet for the internal only machines
* Images of Ubuntu server 10.04.4 LTS and 12.04 LTS

=== Future ===
Upcoming, and nice to have for the current migration:
* Internal DNS
** Note: We currently spreading a ''hosts'' file with Salt stack
* Private network to communicate with all the instances
** VPN between sites (iWeb site and Dreamhost site)
* Object storage service (Swift/Ceph or similar; not in use, but planned)
** Note: our server setup is using Gluster FS and we are considering switching to use OpenStack's Swift/Ceph to store our static assets.

=== Next year ===
* MySQL cluster to be upgraded, multiple site replication
* Implementing continuous deployment, configuring states on a local development machine using Vagrant/VirtualBox, test deployment script in staging/test, then deploy in production.
* Log management analysis tool to help us audit system symptoms
* We plan to leverage [http://en.wikipedia.org/wiki/Edge_Side_Includes ESI] ("Edge Side Include") for some aspects of the site content.