== Summary ==
Collection of small shell scripts that will be used to test components of the infrastructure.

== By technology ==
=== PHP Memcache library connection to Memcache cluster ===

    $params = array(
             'class'      => 'MemcachedPeclBagOStuff',
             'serializer' => 'php',
             'servers'    => array(
                     '10.1.1.1:11211',
                     '10.2.2.2:11211',
             ),
             'timeout' => 250000,
             'connect_timeout' => 300
    );
    $client = new Memcached;
    $client->setOption( Memcached::OPT_CONNECT_TIMEOUT, $params['connect_timeout'] * 1000 );
    $client->setOption( Memcached::OPT_SEND_TIMEOUT, $params['timeout'] );
    $client->setOption( Memcached::OPT_RECV_TIMEOUT, $params['timeout'] );
    $client->setOption( Memcached::OPT_POLL_TIMEOUT, $params['timeout'] / 1000 );
    $client->setOption( Memcached::OPT_LIBKETAMA_COMPATIBLE, true );
    $client->setOption( Memcached::OPT_SERIALIZER, Memcached::SERIALIZER_PHP );
    //require('/srv/webplatform/wiki/current/includes/GlobalFunctions.php');
    require('/srv/webplatform/wiki/current/includes/IP.php');
    //require('/srv/webplatform/wiki/current/includes/objectcache/MemcachedPeclBagOStuff.php');
    $servers = array();
    foreach ( $params['servers'] as $host ) {
        $servers[] = IP::splitHostAndPort( $host ); // (ip, port)
    }
    $client->addServers( $servers );
    $tmp_object = new stdClass;
    $tmp_object->str_attr = 'test';
    $tmp_object->int_attr = 123;
    $tmp_object->date = new DateTime();
    $client->add('key1', $tmp_object, 10) or die ("Failed to save data at the server");
    var_dump($client->get('key1'));
    var_dump($client->get('wpwiki:user:stats:359'));


=== Website vhost ===

* One per vhost
* Grep if a string exist
* Return non zero if it fails
* See for [http://nagiosplugins.org/man/check_http Nagios check_http]

<syntaxHighlight>
    #!/bin/bash
    curl -I -H 'Host: docs.webplatform.org' http://15.185.116.171/wiki/Main_Page?t=cli-renoirb
</syntaxHighlight>


=== Adding pages through MediaWiki API ===

'''Dependencies''':
* Varnish configuration do not send cached documents as a reply to a POST request, see [[WPD:Infrastructure/procedures/Maintaining Varnish or Fastly configuration]]

<syntaxHighlight lang="bash">
#! /bin/sh
#
# author: Max Polk
#
echo "TEST connecting to a wiki and editing using the api.php interface"
 
# Edit these variables
export WIKI_USERNAME='ZZZ'
export WIKI_PASSWORD='ZZZ'
export WIKI_API='http://docs.webplatform.org/t/api.php'

# Under mac OS, option dry-run doesn't exist, you can do `cat temporaryfile.txt`  and fill a file with test data
export CONTENT='Sample page contents: '$(mktemp --dry-run)

export PAGE='Tests/javascript-a'
export PAGE_URLENCODED='Tests%2Fjavascript-a'
export SUMMARY='Automated test edit'
export LOG_FILE='LOG.txt'
export RESULT_FILE='RESULT.txt'
export COOKIE_FILE='COOKIES.txt'
 
function append ()
{
    echo "$1" >> "$LOG_FILE"
}
 
function appendfile ()
{
    cat "$1" >> "$LOG_FILE"
}
 
function showbanner ()
{
    echo
    echo "----------------------------------------------------------------------"
    echo "$1"
    echo "----------------------------------------------------------------------"
}
 
function showoutput ()
{
    cat "$LOG_FILE"
}
 
#======================================================================
# Login
#======================================================================
 
# New log file for this request
showbanner "Login request"
echo -n > "$LOG_FILE"
 
# Empty the cookie file
echo -n > "$COOKIE_FILE"
append "EMPTIED cookie jar"
append ""
 
# Post request
append "POST to $WIKI_API"
append ""
append "PARAMETERS:"
append "    action=login"
append "    lgname=$WIKI_USERNAME"
append "    lgpassword=$WIKI_PASSWORD"
append "    format=json"
append ""
curl -s --show-error -i "$WIKI_API" -d action=login -d "lgname=$WIKI_USERNAME" -d "lgpassword=$WIKI_PASSWORD" -d format=json -b "$COOKIE_FILE" -c "$COOKIE_FILE" > "$RESULT_FILE"
append "HTTP dump:"
append ""
appendfile "$RESULT_FILE"
append ""
append ""
 
# Verify last result
if ! grep -q '"result":"NeedToken"' "$RESULT_FILE"; then
    append ""
    append 'FAILURE, did not find: "result":"NeedToken"'
    append ""
    append 'EXPECTED something like: {"login":{"result":"NeedToken"'
    showoutput
    exit 1
fi
# Get token from last result
export TOKEN=$(grep "^{" "$RESULT_FILE" | sed 's/^.*"token":"\([^"]*\)".*$/\1/')
if [ -z "$TOKEN" ]; then
    echo "Unable to find token"
    exit 1
fi
append ""
append "EXTRACTED TOKEN:"
append "    $TOKEN"
showoutput
 
#======================================================================
# Verify login using login/token from previous output
#======================================================================
 
# New log file for this request
showbanner "Login verification"
echo -n > "$LOG_FILE"
 
# Post verification
append "POST to $WIKI_API"
append ""
append "PARAMETERS:"
append "    action=login"
append "    lgname=$WIKI_USERNAME"
append "    lgpassword=$WIKI_PASSWORD"
append "    lgtoken=$TOKEN"
append "    format=json"
append ""
curl -s --show-error -i "$WIKI_API" -d action=login -d "lgname=$WIKI_USERNAME" -d "lgpassword=$WIKI_PASSWORD" -d "lgtoken=$TOKEN" -d format=json -b "$COOKIE_FILE" -c "$COOKIE_FILE" > "$RESULT_FILE"
append "HTTP dump:"
append ""
appendfile "$RESULT_FILE"
append ""
append ""
 
# Verify last result
if ! grep -q '"result":"Success"' "$RESULT_FILE"; then
    append ""
    append 'FAILURE, did not find: "result":"Success"'
    append ""
    append 'EXPECTED something like: {"login":{"result":"Success"'
    showoutput
    exit 1
fi
 
append ""
append "SUCCESSFULLY VERIFIED LOGIN"
showoutput
 
#======================================================================
# Get an edit token
#======================================================================
 
# New log file for this request
showbanner "Obtain edit token"
echo -n > "$LOG_FILE"
 
# Query for edit token
append "GET from $WIKI_API"
append ""
append "PARAMETERS:"
append "    action=query"
append "    prop=info"
append "    intoken=edit"
append "    titles=${PAGE}"
append "    format=json"
append ""
append "ACTUAL URL:"
append "    ${WIKI_API}?action=query&prop=info&intoken=edit&titles=${PAGE_URLENCODED}&format=json"
append ""
curl -s --show-error -i "${WIKI_API}?action=query&prop=info&intoken=edit&titles=${PAGE_URLENCODED}&format=json" -b "$COOKIE_FILE" -c "$COOKIE_FILE" > "$RESULT_FILE"
append "HTTP dump:"
append ""
appendfile "$RESULT_FILE"
append ""
append ""
 
# Verify last result
if ! grep -q '{"query":{"pages"' "$RESULT_FILE"; then
    append ""
    append 'FAILURE, did not find: {"query":{"pages"'
    append ""
    showoutput
    exit 1
fi
 
# Get edit token from last result (unescape JSON "\\" into "\")
export EDIT_TOKEN=$(grep "^{" "$RESULT_FILE" | sed 's/^.*"edittoken":"\([^"]*\)".*$/\1/' | sed 's/\\\\/\\/g')
if [ -z "$EDIT_TOKEN" ]; then
    echo "Unable to find edit token"
    exit 1
fi
append ""
append "EXTRACTED EDIT TOKEN:"
append "    $EDIT_TOKEN"
showoutput
 
#======================================================================
# Perform actual page edit
#======================================================================
 
# New log file for this request
showbanner "Perform page edit"
echo -n > "$LOG_FILE"
 
# Post edit
append "POST to $WIKI_API"
append ""
append "PARAMETERS:"
append "    action=edit"
append "    title=${PAGE}"
append "    summary=${SUMMARY}"
append "    text=${CONTENT}"
append "    bot=1"
append "    watchlist=nochange"
append "    token=${EDIT_TOKEN}"
append "    format=json"
append ""
curl -s --show-error -i "${WIKI_API}" -d action=edit -d "title=$PAGE" -d "summary=$SUMMARY" -d "text=$CONTENT" -d bot=1 -d watchlist=nochange --data-urlencode "token=$EDIT_TOKEN" -d format=json -b "$COOKIE_FILE" -c "$COOKIE_FILE" > "$RESULT_FILE"
append "HTTP dump:"
append ""
appendfile "$RESULT_FILE"
append ""
append ""
 
# Verify last result
if ! grep -q '"result":"Success"' "$RESULT_FILE"; then
    append ""
    append 'FAILURE, did not find: "result":"Success"'
    append ""
    append 'EXPECTED something like: {"login":{"result":"Success"'
    showoutput
    exit 1
fi
 
showoutput
 
#======================================================================
# Logout
#======================================================================
 
# New log file for this request
showbanner "Logout"
echo -n > "$LOG_FILE"
 
# Post logout
append "POST to $WIKI_API"
append ""
append "PARAMETERS:"
append "    action=logout"
append "    format=json"
append ""
curl -s --show-error -i "$WIKI_API" -d action=logout -d format=json -b "$COOKIE_FILE" -c "$COOKIE_FILE" > "$RESULT_FILE"
append "HTTP dump:"
append ""
appendfile "$RESULT_FILE"
append ""
append ""
 
# Verify last result
if ! grep -q "\[\]" "$RESULT_FILE"; then
    append ""
    append "FAILURE, did not find: \[\]"
    append ""
    showoutput
    exit 1
fi
 
append ""
append "SUCCESSFULLY LOGGED OUT"
showoutput
 
#======================================================================
# Success
#======================================================================
 
showbanner "SUCCESS"
</syntaxHighlight>