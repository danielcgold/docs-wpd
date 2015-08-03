---
title: WPD:Community/Meetings/General/2013/1122 raw mtg notes
---
<p>scribenick: jkomoros
</p><p>topic: HTML Elements
</p><p>q+
</p><p>eliot: Happy to be coordinator on it, in parallel to JS work. important to move forward with a regular heart beat, have WPW on them, etc
</p><p>shepazu: I think this is a great idea. It's also conspicuous that we don't have them. this content is the kind of stuff that you can find anywhere but people see we don't have HTML, and then are disappointed
</p><p>eliot: When we did the CSS font property page as an example? we should do the same thing for a representative HTML Element and Attribute
</p><p>jensimmons: I'd be happy to work on that looking to help with a design. Imaginging: what's it like to be a student, etc, do people understand the page? not visually, but in terms of content. could do a study of how other successful sites are doing it
</p><p>shepazu: That's how we approached CSS that sounds like a great plan
</p><p>ACTION: eliot to create example attribute/element pages
</p><p>maxpolk: There's convergence between elements, apis, etc there are side links between various pages
</p><p>eliot: That's how it is in the specs as well
</p><p>topic: Dave Gash is working on reorg of HTML DOM API
</p><p>dgash: The main thrust is we have 100's or maybe even 1000's of pages that have been imported to long URLs with things like "events" "properties" etc that aren't necessary geting rid of interstitials and moving them to where they sit done this under dom node, and audio/video, and in th emiddle of traversal the end result of this that the pages will be in a more logical order and available for review and editing still have quite a few to go, but that's what I'm working on at the moment.
</p><p>julee: Eliot's primary project is to get the pages themselves done we've lost some momentum on the actual content creation, want to help bring in contributors again
</p><p>shepazu: A few peopel has asked me, when will WPW start back again?
</p><p>eliot: As soon as we have a page template
</p><p>jensimmons: My other projects will wrap up soon, so I can get started on this next week
</p><p>maxpolk: There's an html elements effort, right? there's a form, for example
</p><p>eliot; And we imported elements from MSDN it just needs to be reviewed and given best practices
</p><p>julee: We like to have a golden example to refer to
</p><p>jensimmons: It seems like the structure of the content was originally based on the import, but this would be a good time to rethink some of the organization?
</p><p>shepazu: Absolutely
</p><p>eliot: We did SOME of it back at the import
</p><p>jkomoros: Yeah, we made an effort
</p><p>eliot: So it needs some work, but there's a bit of structure there already
</p><p>shepazu: And we should never stop thinking about how we can improve the pages
</p><p>maxpolk: We should try to automate what we can
</p><p>agenda: CSS Compat tables
</p><p>julee: Last time someone had done client side stuff and it was getting ready for testing?
</p><p>shepazu: renoirb deplohyed on the test wiki the extension he said it seemed to work, but we need to put it through its paces
</p><p>Hey hi the other part of the problem is collecting data Ronald Mansfeld started very enthusiastically but he has lost a bit of momentum a few weeks ago haven't heard from him in awjhile I just e-mailed him last night Ronald has designed a data model and started pulling the data from MDN but he hasn't responded recently I tried e-mail, now I'll try contacting other people who might know him worst case we'll have to start again from the json data model on github
</p><p>renoirb: Regarding the extension for compat tab les, it's likely a problem with varnish caching; but it's working in the test instance so I just need to adjust the way the tag is written
</p><p>ESI tags can be seen here <a rel="nofollow" class="external free" href="http://docs.webplatform.org/test/Tests/Compatibility_table_and_caching">http://docs.webplatform.org/test/Tests/Compatibility_table_and_caching</a>
</p><p>ACTION: shepazu and renoirb to figure out how well the compat table extension is working; lock it down
</p><p>renoirb: I also started talking to fastly people, and they supported me.
</p><p>Topic: Js Import
</p><p>maxpolk: I believe renoirb fixed the import bug
</p><p>renoirb: Yeah, there was some missing part in the caching. It's basically fixed.
</p><p>maxpolk: So now I'm unblocked for importing JS into the test wiki this includes the changes to the URL scheme it's evolutionary, it's just to have a look at how it feels I dropped it for a bit when it went idle, but now it's my top priority again
</p><p>shepazu: Max and I met in person and hashed some stuff out over dinner and coffee and we sorted out that this should be a iterative process it's not done yet. like, for example we don't have templates for these. we're going to need to make templates, just regular wiki markup phase 1 is us taking a look at it jensimmons , this is another part where looking at other successful sites for JS reference
</p><p>eliot: I'd like to urge a sense of urgency. I'm getting questions from the team who donated about when it will show up presumably seeing it on the test wiki would be a step in the right direction
</p><p>maxpolk: It should be in the next couple of days I came have it up. but some of the text will need work; like things that are IE specific
</p><p>eliot: We can handle that in manual review, too.
</p><p>maxpolk: Conceptually the templates aren't hard to output to
</p><p>shepazu: Does anyone have time/expertise in making expertise tempaltes
</p><p>maxpolk: Ideally you look at page content before coming up with templates?
</p><p>jensimmons: Should I focus on HTML or JS first?
</p><p>(everyone murmurs agreement about JS)
</p><p>julee: I started a thread on this back in the day so there's some info out there getting some ECMAScript people to help work through it that would really help as well I know shepazu contacted some folks before maybe we could all reach out to our favorite JS expert and ask for their opinion on these threads
</p><p>shepazu: Another thing that might help is for us to all compile a list of JS doc pages that we like to help seed that
</p><p>jensimmons: I'll do at a competitive analysis fo other docs sites, but also what other resources do devs use? and talk to some real developers with the goal of making something BETTER
</p><p>shepazu: It doesn't have to be perfect to start, we can keep iterating
</p><p>jensimmons: Yeah, I'll do it as quickly as I can
</p><p>Topic: How was TPAC?
</p><p>Topic: (As well): Universal Access pointers
</p><p>eliot: Doug and I did a breakout session on WPD lightly attended, but good representative group and good discussion Brian Sullivan from AT&amp;T pointed out a lack of mobile content Cynthia Shelly from Microsoft is working with W3C taskforce on accessibility Larry Masinter talked about areas of deep knowledges--where beginner and intermediate developers wouldn't go we had outreach by at least two peopel who have tools to grab API information from specs and turn it into content
</p><p>julee: By the way, I work with a slightly different Larry than the one you talked to
</p><p>maxpolk: I thought the automation was curious is that even a reasonable possibility for JS, going to ECMA
</p><p>eliot: The tools currently point at W3C specs but dom on W3C tool is looking at the Khronos WebGL spec as well it woudl be difficult to port over all the WebGL stuff by hand lots of goodness that could potentially come out of this tool
</p><p>shepazu: There were other good side conversations there I talked to a few guys from GitHub they are investigating W3DC
</p><p>s/W3DC/W3C I had good conversations about CMS stuff with them also had good conversations with Akamai (one of the biggest CDNs) they collect really good stats on browser usage and content usage maybe they could expose those stats via WPD
</p><p>eliot: Richard Ashida requestsed that we make available for each templated topic a section on universal accessibility (internationalization and accessibility)
</p><p>s/Ashida/Ishida/
</p><p>shepazu: Basically the idea would be a section that links out to other resources about accessibiltity and internationalization in the future getting it folded into content but for now having each page point to good docs for that specific topic would be a good start
</p><p>eliot: This would be hidden unless it has content in it
</p><p>shepazu: We'd need to change the template of all of the pages to include Universal Access
</p><p>eliot: We told him, we're strapped for resources, so can't do this in the near future
</p><p>ACTION: shepazu to talk to MediaWiki folks and see if someone can help with templates
</p><p>shepazu: Another piece of feedback someone thought we needed to have more stubs so that there could be all of the relevant links, and then fill it in as we have the time and energy we've talked about this before: a master list of content we know we want I think there's value in that different contributors might have different interests and not be interested in our main push project at the moment
</p><p>julee: I want to have a clear UI experience for a page ready for consumption vs page that's in progress we've also talked about consolidating flags into one alert icon or something having the whole structure would be good in that case but if we have tons of pages but with no differentiation it could lead to confusion
</p><p>jensimmons: As a new person to the site, I'm confused when surfing around the site
</p><p><br />
</p><p>agenda: Status on migration
</p><p>s/agenda/topic
</p><p>renoirb: I need to sync with ryan about making a copy of the database so no news yet on the real meat
</p><p>shepazu: I'll push the issue with DH today renoirb and ryan will work to be ready to go when DH pushes the button it would be good to talk to Ryan today if we can. The ideal time to pause is probably late at night on a weekend
</p><p>eliot: So next meeting is two weeks from today, right?
</p><p>Thanks, jkomoros!
</p><p>Meeting over
</p>
<!-- Saved in parser cache with key wpwiki:pcache:idhash:12858-0!*!*!*!*!*!*!esi=1 and timestamp 20150731184850 and revision id 41846
 -->
