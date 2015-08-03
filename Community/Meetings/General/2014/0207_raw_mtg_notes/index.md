---
title: WPD:Community/Meetings/General/2014/0207 raw mtg notes
---
<pre>  jkomoros_
</pre>
<p>scribenick: jkomoros_
</p><p>topic: MDN Compat Tables
</p>
<pre>  jentesting
</pre>
<p>I won't be on the phone today, but I'll lurk in this channel if my tethered phone connection says working. This is Jen Simmons, btw.
</p>
<pre>jkomoros_
</pre>
<p>shepazu: frozenice made a script to pull in data from MDN
</p><p>... renoirb made a conversion script from that format into more clean data
</p>
<pre>renoirb
</pre>
<p>is sorry to be late
</p>
<pre>jkomoros_
</pre>
<p>... we're using MDN as the starting point for compat data, since it's tehc loest match to our page structure.
</p><p>... using the caniuse json format to format the JSON
</p><p>... later we'll work with our own data format that will be able to accomodate data from our sources
</p><p>... but this is an easy first pass
</p><p>... next we should be able to work on the medaiwiki extension that takes the json and injects into web pages
</p><p>... uses something like this format
</p><p>... we're going to modify that script slightly to work with the new data
</p><p>... then I think we're good to put this data out
</p><p>renoirb: There's some limitations on the script that frozenice mentioned
</p><p>... trying to understand it, but basically it doesn't fetch all because of limitations on paginations on kuma
</p><p>... so we might need to dig a bt deeper on that
</p><p>shepazu: Might have to do with ratelimiting
</p>
<pre>renoirb
</pre>
<p>Look at the "Current issues" <a rel="nofollow" class="external free" href="https://github.com/webplatform/mdn-compat-importer/blob/master/README.md#current-issues">https://github.com/webplatform/mdn-compat-importer/blob/master/README.md#current-issues</a>
</p>
<pre>jkomoros_
</pre>
<p>... the big thing is that we have a working conversion script
</p><p>renoirb: This link ^ has information on the current issues
</p><p>... so it's probably not all data, but we can compare later when we can get more
</p><p>karlcow [~karl@nerval.la-grange.net] entered the room.
</p>
<pre>jkomoros_
</pre>
<p>jkomoros_: Is this a run-once-and-never-again kind of thing?
</p><p>shepazu: We've been assumign we're going to run it once
</p><p>... MDN data isn't updated all of that often
</p><p>... renoirb wrote a rigorous script (with frozenice ), so if we need to, we can run it again
</p><p>jkomoros_: I was more thinking, if we work on the data, later imports could blow it away
</p><p>shepazu: I wish jswisher were here today, but we'd love to work closer with MDN
</p><p>... there's room for improvement in the data, especially when we merge in caniuse
</p><p>... we could have different data sources all munged into one data source
</p><p>... we're going to do that with caniuse and W3C test suite anyway
</p><p>... we could store our own updated data in a separate store and then merge those on
</p><p>... so our data would take precedence over MDN (likely)
</p><p>... make all the data available via the same API from multiple sources
</p><p>shepazu: Jeremie Pationnier (sp?) is driving an effort in MDN to improve their compat tables data
</p><p>... they weren't aware of this project. We'll make the normalized data available to them, obviously
</p><p>... to help them structure their data more consistently. Hopefully we can convince the MDN folks to join forces with this project
</p><p>hyperair left the room (quit: Ping timeout: 245 seconds).
</p>
<pre>jkomoros_
</pre>
<p>jkomoros_: That could be difficult in practice, but if it works, great!
</p><p>shepazu: I'll reach out to MDN folks about what we're doing, our next steps, our current status, etc on Compat tables
</p><p>... I'm going to try to work on the script (working with renoirb) over the next week to try to get the script (the extension for mediawiki) going
</p><p>... will also work with ryanlane
</p><p>... hopefully we'll have, by next friday, the compat table information generated and displayed in the site
</p><p>[much rejoicing]
</p><p>... after that, major blocker for announcing CSS prop project is the ready/not-ready flag
</p><p>... we have the groundwork laid for that so hopefully it won't be too challenging
</p><p>... eliezerb already wrote the template for that
</p><p>... and then we need to start talking about how to make the announcement
</p><p>topic: WPW for JS
</p><p>shepazu: since jen isn't here we can't talk about home page effort
</p><p>... so I think the rest of this meeting should be about JS WPW
</p><p>... eliot helped drive a blog post from maxpolk about JS and the community
</p><p>... I thought it was very nicely done
</p><p>... we now have the JS stuff imported
</p><p>... and have WPW coming up.
</p><p>julee__:
</p><p>... this week I tried to get folks to contribute to the Gold Standard JS page
</p>
<pre>renoirb
</pre>
<p>julee: I did a little bit  
</p>
<pre>jkomoros_
</pre>
<p>... no one volunteered. I did some work and then requested that folks contribute examples, and no one stepped up
</p><p>... eliot added a sub-agenda item about what's the plan
</p><p>...we have everything set up, we just need to have contributors and coordinators
</p><p>... I'm a little hesitant about what will happen next week, since no one has stepped up yet
</p><p>... maybe if we can have some of us on this phone call volunteer to coordinate
</p><p>... and maye amplify the blog post
</p><p>... and tweet
</p><p>... to get some folks back into the fold
</p><p>shepazu: I think there's a matter of bringing more people into the fold
</p><p>... the people who care about JS might be different than the ones who helped out with WPW for CSS
</p><p>... maybe we should have two WPW's running: JS and HTML at the same time?
</p>
<pre>jkomoros_
</pre>
<p>julee: Given that we can't find enough for one, I think we should just focus on JS
</p>
<pre>jkomoros_
</pre>
<p>eliot: We need to walk before we run
</p><p>... the bottleneck now is getting it going, and JS is the priority above HTML
</p><p>... if we have momentum from that we can look at also kicking off JS
</p><p>... I agree that audiences are different potentially
</p><p>shepazu: I think it will be harder to find JS people to contribute than HTML people to contrbute
</p><p>... so it seems harder to start on JS than HTML
</p>
<pre>jkomoros_
</pre>
<p>julee: i see that as well
</p>
<pre>jkomoros_
</pre>
<p>... I was being firm on JS project since we had excitement about it this summer and had announced our intention
</p><p>... but I'm willing to reassess
</p><p>eliot: I think you're both right but [scribe was asleep at the wheel for a minute]
</p><p>shepazu: so maybe we start more modestly as we ramp up. we have say 5 people
</p><p>... maybe we do 5 JS pages a week to start (or maybe 10) and build up a base of contributors that way
</p><p>... I'm concerned with having a gap if we aim too high (like 20), that could have us lose momentum
</p><p>... maybe if we shoot for 5 and ramp up as capacity increases
</p>
<pre>jkomoros_
</pre>
<p>julee: I'm less worried about numbers than having hte commitment to be coordinators
</p>
<pre>jkomoros_
</pre>
<p>... and do the community work to pull folks in
</p><p>shepazu: Filling out reference pages is easy but boring
</p><p>... what if we tried to pair (or gave as an option) take a reference page, and also consider writing a longer article/tutorial about using the feature
</p><p>... there might be some peopel that woudl appeal to
</p><p>jkomoros_: My gut is that's more work for them to do, making it less likely
</p>
<pre>jkomoros_
</pre>
<p>julee: But making the work more interesting is a good idea
</p>
<pre>jkomoros_
</pre>
<p>shepazu: So maybe we need to highlight the more interesting aspects
</p><p>Jeremie [~Jeremie@89.202.203.52] entered the room.
</p>
<pre>jkomoros_
</pre>
<p>eliot: I think that's what came out in the CSS props project: people liked the example code bits best
</p><p>julee__: And if there are good examples on the page, then people who are less knolwedgable can pull from those to write reference
</p><p>... this week when I tried to get people involved I asked fo rpeople to write examples
</p><p>shepazu: I don't think I could write a good article on JS
</p><p>... I could do it for SVG or HTML or CSS
</p><p>... JS feels like it has a higher bar for quality
</p>
<pre>renoirb
</pre>
<p>q+
</p><p>shepazu, julee__
</p><p>Go ahead Eliott
</p>
<pre>jkomoros_
</pre>
<p>eliot: What I say at doc sprints to that: "we're nto writing the definitive book, we're writing a wiki"
</p><p>... others can come to edit/contribute/amend
</p><p>... we're not shooting for perfect, but solid
</p><p>shepazu: I still feel like JS is harder
</p><p>... and that there will be others like me who are intimidated
</p><p>renoirb: How about some of us take some time looking at good blogs/sites and ask them to help?
</p><p>... and JS communities to contact
</p><p>shepazu: What's the timing on all of this?
</p>
<pre>jkomoros_
</pre>
<p>julee: I outlined in the blog post that we'll release the pages on tuesday nights
</p>
<pre>jkomoros_
</pre>
<p>... and blog post specifically mentioned next tuesday
</p><p>ACTION: everyone to share the blog post about JS WPW and contact people in their community to amplify and join
</p><p>[renoirb, eliot, shepazu commit to being coordinators]
</p>
<pre>jkomoros_
</pre>
<p>julee: Process can be same as before
</p>
<pre>jkomoros_
</pre>
<p>... once people know what they're doing we can have people volunteer to coordinate
</p><p>... plan was to get import done in Jan, WPW in Feb, and then we have the fluentconft
</p><p>... where there are a lot of folks who can join us
</p><p>... then the docsprint in... belgium?
</p><p>shepazu: Isn't that on hold?
</p><p>julee__: After the docsprint in march we can assess if we're getting enough contributors, how it's going, or if we should move over to HTML
</p><p>eliot: What about having HTML ready for fluent?
</p><p>... to leverage that expertise there?
</p><p>shepazu: That seems reasonable
</p>
<pre>jkomoros_
</pre>
<p>julee: I thought fluent was more about JS developers
</p>
<pre>jkomoros_
</pre>
<p>eliot: I think it will be both
</p>
<pre>jentesting
</pre>
<p>Fluent used to be about JS only, but they are pushing hard to make it Web Platform in general
</p>
<pre>jkomoros_
</pre>
<p>shepazu: Just want to make sure we don't turn people away who don't want to do JS
</p>
<pre>jentesting
</pre>
<p>and yes, the Belgium doc sprint doesn't have any dates. April was proposed, but won't work.
</p>
<pre>jkomoros_
</pre>
<p>eliot: I'm willing to drive that effort to get ready for HTML by then
</p>
<pre>jkomoros_
</pre>
<p>julee: and I can help as well... I just don't know if we have enough consistent community management to be able to handle both
</p><p>_cheney left the room (quit: Read error: Connection reset by peer).
</p><p>_cheney [~cheney@nat.sierrabravo.net] entered the room.
</p><p>mode (+o _cheney) by ChanServ
</p>
<pre>jkomoros_
</pre>
<p>eliiot: I think most important is getting the golden example pages for element + attribute
</p>
<pre>jkomoros_
</pre>
<p>julee: I'm okay with that
</p>
<pre>jkomoros_
</pre>
<p>... especially given the number of peopel who will be there
</p><p>eliot: I'll be there, too
</p><p>... docsprint is open to public
</p><p>shepazu: So we have a plan to announce and what we'll be doing
</p><p>eliot: I'm sitll a little unclear about this coming week's
</p><p>shepazu: My perception is that we have a: we work on a blogpost and each of us tries to find at least one expert to volunteer
</p><p>julee__: The blgopost is already out to point people at
</p><p>... sot he idea is to announce that the WPW will start next wek
</p><p>... and send out to folks
</p><p>... on tuesday we should have a blog post about the topics for the first week
</p><p>... I was going to start with Array and see who shows up
</p><p>shepazu: MDN has excellent JS docs
</p><p>... maybe we should see if people who contributed there would be interested in being involved
</p><p>ACTION shepazu to reach out to MDN folks who contributed to JS documentation and see if they want to be involved in JS WPW
</p>
<pre>renoirb
</pre>
<p>wants to have your feeling about <a rel="nofollow" class="external free" href="http://www.w3.org/mid/2703272A-5C27-4FDE-A62A-7133307BE3D2@w3.org">http://www.w3.org/mid/2703272A-5C27-4FDE-A62A-7133307BE3D2@w3.org</a>
</p><p>AGENDA+ ^
</p>
<pre>jkomoros_
</pre>
<p>[scribe was distracted for a few minutes]
</p><p>shepazu: I think to keep the community we need to keep up the engagement
</p><p>... short term we just need to find people to help with JS stuff
</p><p>ACTION: shepazu to create a doodle poll about moving this meeting
</p>
<!-- Saved in parser cache with key wpwiki:pcache:idhash:15624-0!*!*!*!*!*!*!esi=1 and timestamp 20150731185017 and revision id 46241
 -->
