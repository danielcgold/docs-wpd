Among Web Platform Docs features is a live code viewer and pastebin. It allows us to keep in one place all code samples.

The webapp we are using for this is [http://lea.verou.me Lea Verou]'s [http://dabblet.com/ Dabblet] available at [http://code.webplatform.org/ '''code.webplatform.org'''] and keeps the code in a [https://gist.github.com/WebPlatformDocs dedicated GitHub Gists repository].

==Features==
* Provides a live preview of input HTML, CSS, SVG, JavaScript, etc. ''(mostly done)''
* Allows users to share code snippets with each other, as a pastebin ''(mostly done, still replies on GitHub)''
* Provides a way to open example code from the wiki in live example without copy-paste ''(some progress, not done)''

==Integration==
Because integration has many aspects, we will roll out full support for this feature in several steps.

===Roadmap===
====Phase 1: Static Live Code Viewer====

'''Status:''' ''Done''

====Phase 2: Open Examples from Wiki====

'''Status:''' ''not started''

====Phase 3: Inline Live Examples====

'''Status:''' ''not started''

====Phase 4: Host Gists on WebPlatform.org====

'''Status:''' ''not started''

===Other Tasks===

==Technical Requirements==
===Dedicated Subdomain===
The public URL will be [http://code.webplatform.org code.webplatform.org].

===Additional Subdomains===
In addition to the public-facing URL, Dabblet needs two additional subdomains for security reasons:
* '''Result preview:''' This is only used internally and not displayed to the user. It's a separate domain for security reasons, otherwise people could write dabblets that leak the user's access token. On dabblet.com, this is called preview.dabblet.com
* '''Full-page results:''' This is for results without any dabblet chrome around them. Separate subdomain for the same security reasons. On dabblet, this is result.dabblet.com. This is not critical, worst case we could just disable this feature.

==== Why are separate subdomains needed? ====
localStorage is local per subdomain. In dabblet, localStorage stores the user’s Github access token. An access token is a unique string Github Oauth sends to dabblet after authentication is succesfull, to identify the current user, and dabblet uses that token in subsequent requests. If executed scripts had access to dabblet’s localStorage info, they could steal the current user’s access token and send it to an arbitrary server so some attacker could use it to log in to Github as the dabblet user that access token belonged to.

=== Github API keys ===
https://github.com/organizations/webplatform/settings/applications/34604

=== File edits required ===
* code/global.js for Client API key (Done)
* Rename sample.oauth.php to oauth.php
* oauth.php for domain and Client & Secret API keys (Done)
* HTML and JS files, for the domain
* Change .htaccess with the proper domain and subdomains (Partially done)

=== Git ===
Github repo: https://github.com/webplatform/dabblet

TODO: Need to be able to have separate git subdirectory with the above as a remote, so we can easily pull changes. Might be a problem if we have a different structure for the subdomains (i.e. completely separate files instead of subfolders).

=== Deploy ===
salt-run deploy.run code.dabblet

== Branding ==

* Logo
* Skinning (colors etc)
* Prism theme (will also be used on WPD)
* Links to WPD sections