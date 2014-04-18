= OAuth Study notes =

See [http://notes.webplatform.org/stream?tags=gist-9837155 annotations thread].

== What is OAuth? ==

OAuth is a way to validate authenticity between various players in the context of multiple application communicating together. It is a framework to validate the rights ("grant") and how to request ("scope", "entitlements") for information ("resource") from one system to another.

While the name OAuth has "auth" in it, it is commonly confused with "Authentication" but, in fact, its about "Authorization. 

In other words, OAuth isn’t about proving who you are, but to provide verification mechanism based on a key token (i.e. Bearer token) generated by previous authentication. Each Relying parties that accept OAuth can use the OAuth server and double check if the given token is still valid. If the token is not, it will forward the user to the defined authentication service. 

'''Note''': You can read [http://merbist.com/2012/04/04/building-and-implementing-a-single-sign-on-solution/ Building and implementing a Single Sign On Solution] article, it explains well the confusion with SSO and OAuth and our objective toward SSO and the use of OAuth.

OAuth is similar to what a ''Valet-key'' of a car is for:
<blockquote> 
Many luxury cars come with a valet key. It is a special key you give the parking attendant and unlike your regular key, will only allow the car to be driven a short distance while blocking access to the trunk (...).
</blockquote> 
source (link10)

OAuth is not the first attempt to solve the authentication. There were also OpenID, and SAML, both are older and besides the fact that OAuth is younger, it can do more. 

While OpenID was about keeping authorization and user information. It doesn’t solve the problem that third parties has to create a local account with the user. That's where OAuth comes in to play.

* Giving access tokens to consumers without giving away private information
* Setting ''rules'' for sharing information through APIs
* Keywords:
** '''Service provider''': It is understood that this is used when an entity serves both as: Resource Server, and Authorization server in the transparently.
** '''Resource server''': The API; (''synonyms'': RS)
** '''Authorization server''': The system to login against; (''synonyms'': AS)
** '''Consumer''': 3rd party looking to receive data. (external site, mobile app, etc)
** '''User''': A human being (''synonyms'': Ressource owner)
** '''Scope''': Expressed in non standardized ways, to convey what can be done. (''synonyms'': entitlement)
** '''Grant''': Many types, depending of the use-case (''synonym'': Flow) see (link9), (link10)
* To serve as a way to certify what is allowed to be done, before doing it. The part that is describing is referred to as "Scope" or "Entitlement" (link2)
* Ways to describe Scope/entitlement spec leaves it open ended. In the article (link2) they show various ways used by know websites.

=== In other words ===

<blockquote>
The client application obtains a token (with user consent) with which the client application can act on behalf of a user. Note the important distinction: the application does not become the user. The application is simply able to indicate that it is acting on behalf of a user for a particular scope of activity.
</blockquote>
[http://notes.webplatform.org/a/D3xZP4xeTpiKDFHD_IGrFA annotation], source: (link6)


=== Compared to SAML ===
Both address the same problem, besides the fact that SAML is dating from 2005 and serves only to web applications. In other words, due to SAML design, a native mobile application cannot use it. Because back in 2005, nobody could expect the mobile bubble and the information exchange mechanism requires things that cannot be achieved.


-----

== How OAuth works ==

Quoting the example given in (link8)

[[File:mutuallyhuman-com-strategy-sso-schema-oauth2-flow.png]]

<blockquote>
* (A) – a user opens their web-browser and goes to MyPhotos.com which stores all of their photos. MyPhotos.com doesn't handle authentication itself, so the user is redirected to the Authorization Server with a request for authorization. The user is presented with a login form and is asked if they want to approve the Resource Server (MyPhotos.com) to act on their behalf. The user logs in and they are redirected back to MyPhotos.com.
* (B) – MyPhotos.com receives an authorization grant code as a part of the redirect and then passes this along to the client
* (C) – the Client then uses that authorization grant code to request an access token from the Authorization Server.
* (D) – if the authorization grant code is valid, then the Authorization Server grants an access token. The access token is then used by the client to request resources from the Resource Server (MyPhotos.com).
* (E) – MyPhotos.com receives the request for a resource and it receives the access token. In order to make sure it's a valid access token it sends the token directly to the Authorization Server to validate. If valid, the Authorization Server sends back information about the user.
* (F) – having validated the user's request MyPhotos.com sends the requested resource back to the user.
</blockquote>

If you want to see different use-cases involving various Grant types, the slides at (link12) explains it very well.

-----

== Facts ==

=== Scope ===

Has to be created and enforced among the ecosystem of the OAuth Service provider.

It is basically a set of keywords to describe what information is requested.

For example, when somebody use Twitter as OAuth Service provider, the Consumer can do things that Twitter's scope is allowing. If we create our own OAuth, we have to set in place our ''own'' set of scopes.

Note:
* Some documentation also refer this component as an "Entitlement" (are they synonyms?)
* In SAML, they also have concept of Tokens, but document how to represent it (link8)

==== In other words ====

<blockquote>
(...) because OAuth uses both a client application credential (aka client identifier) and a token representing the user's scope of permission, service providers like banks, are able to set different access policies for client applications authorized by their customers.
</blockquote>
[http://notes.webplatform.org/a/cn5hB9q5SoC9BgnvmoKhdw annotation], source: (link6)

=== Grant types ===

It is unclear in (link10) if he refers as "Flow" is actually what is now known as  "Grant type". I assume that in since 2010 the terminology changed a bit. 

Here is what (link10) described as flow, but summarizes well various "Grant types".

<blockquote>
* '''User-Agent''' –  for clients running inside a user-agent (typically a web browser) (grant_type="'''implicit'''")
* '''Web Server''' –  for clients that are part of a web server application, accessible via HTTP requests. This is a simpler version of the flow provided by OAuth 1.0.   (grant_type="'''authorization_code'''")
* '''Device''' –  suitable for clients executing on limited devices, but where the end-user has separate access to a browser on another computer or device. (grant_type="'''implicit'''")
 * '''Username and Password''' –  used in cases where the user trusts the client to handle its credentials but it is still undesirable for the client to store the user’s username and password.  This flow is only suitable when there is a high degree of trust between the user and the client. (grant_type="'''password'''")
 * '''Client Credentials''' –  the client uses its credentials to obtain an access token. This flow supports what is known as the 2-legged scenario.
 * '''Assertion Flow''' – the client presents an assertion such as a SAML assertion to the authorization server in exchange for an access token.
</blockquote>
source (link10)

=== ''Service provider'', ''Resource Server'' and ''Authorization Server'' ===

There is more than one component

* Resource Server
* Authorization server

Although most of the services expos them as one, they are functionally different and can be decoupled.

'''Synonyms''' (to validate)

* Service provider
* Resource Server ("RS")
* Authorization Server "AS")

=== Tokens, and their lifetime ===

<blockquote>
(...) OAuth uses a code/refresh token/access token system that enables 3 possible session lifetimes for a single relationship (...)
* '''When a user initially authorizes an application''' to have access, a code is issued (first lifetime). Typically this code is used one-time to obtain something called a refresh token or access token.
* '''A refresh token''' (the second lifetime) is '''optional''', but the intention is that it is kept for a longer term and allows the client application to obtain resource access tokens. Refresh tokens might typically last days or months.
* '''Resource access tokens''' (third lifetime) are then used (often as '''bearer tokens''') to access protected services. These tokens are typically short-lived (minutes/hours).
</blockquote>
source: (link6)

'''Synonyms''' (to validate)

* Bearer token
* Token
* Grant
* OAuth Grant
* Authorization

=== SAML vs OAuth ===

This article (link7) went through to compare the terminology and the description of both technologies.

<blockquote>
''SAML'' and ''OAuth2'' use similar terms for similar concepts.

For comparison the formal SAML term is listed with the OAuth2 equivalent in parentheses.

* Service Provider (Resource Server) -- this is the web-server you are trying to access information on.
* Client -- this is how the user is interacting with the Resource Server, like a web app being served through a web browser.
* Identity Provider (Authorization Server) -- this is the server that owns the user identities and credentials. It's who the user actually authenticates with.
</blockquote>
source: (link7)

== And now, for WebPlatform Docs use-cases ==

* ''MediaWiki OAuth Extension'' on [https://github.com/wikimedia/mediawiki-extensions-OAuth github.com/wikimedia] repository and [https://git.wikimedia.org/tree/mediawiki%2Fextensions%2FOAuth the official Gerrit repo].


-----

== References ==

* (link1) [http://www.hongkiat.com/blog/oauth-connect/ Unofficial blog post about OAuth Connect]
* (link2) [http://brandur.org/oauth-scope Unofficial blog post about OAuth Scope] (unofficial article)
* (link4) [http://www.slideshare.net/travisspencer/calling-an-oauth-10a-api-from-an-oauth-20-api Slides about collaboration between multiple OAuth providers]
* (link3) [https://developers.facebook.com/docs/facebook-login/permissions#permissions Facebook developer documentation: OAuth scope and permissions]
* (link5) [https://dev.twitter.com/docs/auth/application-only-auth Twitter developer documentation: Application only auth]
* (link6) [http://www.independentid.com/2010/12/oauth-more-than-just-delegation.html OAuth, more than just delegation]
* (link7) [http://www.mutuallyhuman.com/blog/2013/05/09/choosing-an-sso-strategy-saml-vs-oauth2/ Choosing an SSO Strategy; OAuth vs SAML]
* (link8) [http://en.wikipedia.org/wiki/Security_Assertion_Markup_Language#SAML_Assertions SAML Assertion and tokens]
* (link9) [http://tools.ietf.org/html/rfc6749#section-4.1 IETF OAuth spec, Grant types]
* (link10) [http://hueniverse.com/2010/05/introducing-oauth-2-0/  Introducting OAuth 2.0] (Author: [http://hueniverse.com/author/eran/ Eran Hammer], who participated in the IETF draft of OAuth 1.0)
* (link11) [http://datatracker.ietf.org/doc/active/#oauth Current IETF specs ''Web Authorization Protocol (OAuth)'']
* (link12) [http://www.slideshare.net/aaronpk/an-introduction-to-oauth-2  Slides: An introduction to OAuth 2] (Author: Aaron Parecki, maintainer of OAuth.net)
* (link13) [http://oauth.net/2/ OAuth.net/2/] that is listing various OAuth implementations
* (link14) [http://blog.epanastasi.com/post/56919440376/oauth-is-awesome-oauth-is-horrible OAuth is awesome, OAuth is horrible]!
* (link15) [http://stackoverflow.com/questions/14402938/2-legged-auth-standards-in-2013-should-we-use-oauth2 StackOverflow question: 2-legged auth standards in 2013 -- should we use OAuth2]
* (link16) [http://www.thebuzzmedia.com/designing-a-secure-rest-api-without-oauth-authentication/ Designing a secure API withoug OAuth anthentication]
* (link17) [https://dev.twitter.com/docs/auth/implementing-sign-twitter Twitter developers; A step-by-step example to implement OAuth]
* (link18) [http://merbist.com/2012/04/04/building-and-implementing-a-single-sign-on-solution/ Building and implementing a Single Sign-On solution]