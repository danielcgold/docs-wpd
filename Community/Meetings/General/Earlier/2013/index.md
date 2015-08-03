---
title: WPD:Community/Meetings/General/Earlier/2013
---
<h2><span class="mw-headline" id="Earlier_Web_Platform_general_status_meeting">Earlier Web Platform general status meeting</span></h2>
<p>For the most recent notes on the webplatform.org general status meetings, go to <a href="/wiki/WPD:Community/Meetings/General" title="WPD:Community/Meetings/General">WPD:Community/Meetings/General</a>.
</p>
<h2><span class="mw-headline" id="Agenda_2013-12-06">Agenda 2013-12-06</span></h2>
<ul><li> Jen Simmons has a mock up of the HTML elements pages</li>
<li> Max Polk has done the 3rd JS import</li>
<li> Eliezer Bernart is on templates</li>
<li> David Singer has proposed a WebVTT content project</li></ul>
<h3><span class="mw-headline" id="Raw_meeting_notes">Raw meeting notes</span></h3>
<h2><span class="mw-headline" id="Agenda_2013-11-22">Agenda 2013-11-22</span></h2>
<ul><li> JS import</li>
<li> HTML Elements</li>
<li> CSS compatibility</li>
<li> How was TPAC?</li>
<li> Pointers to info about Universal Access</li>
<li> Migration</li>
<li> Dave's working on DOM re-org</li></ul>
<h3><span class="mw-headline" id="Raw_meeting_notes_2">Raw meeting notes</span></h3>
<p><a href="/wiki/WPD:Community/Meetings/General/2013/1206_raw_mtg_notes" title="WPD:Community/Meetings/General/2013/1206 raw mtg notes">WPD:Community/Meetings/General/2013/1206_raw_mtg_notes</a>
</p>
<h2><span class="mw-headline" id="Agenda_2013-11-08:_Canceled_due_to_lack_of_agenda">Agenda 2013-11-08: Canceled due to lack of agenda</span></h2>
<h2><span class="mw-headline" id="Agenda_2013-11-01">Agenda 2013-11-01</span></h2>
<ul><li> Jen Simmons</li>
<li> TPAC</li>
<li> CSS properties project</li>
<li> Compatibility tables</li>
<li> The next content project?</li>
<li> Status on migration project</li>
<li> Doug will be out the next two Fridays, should we meet anyway?</li></ul>
<h3><span class="mw-headline" id="Discussion">Discussion</span></h3>
<p>julee, shepazu, peterlubbers, jswisher, scottrowe_, jensimmons, renoirb, eliot, patrickdsouza, eliezerb are all on the line or on IRC
</p><p>scribenick: renoirb
</p>
<h4><span class="mw-headline" id="TOPIC:_Jen_Simmons_is_contracting">TOPIC: Jen Simmons is contracting</span></h4>
<p>Good news: Jen Simmons is going to work for at least 6 months or so, starting part time, she is a developer/designer. she is going to be part time for a few weeks and then be full time after she finished her other already planned arrangements.
</p><p>Jen had a chance to talk with a few folks at Html5DevConf, at Google. A lot to work on. Jen is thinking she will work on usability issues and improve it as well as how to help contributors to contribute (making it easier). 
</p><p>Doug believes we should prioritize usability to the users (i.e. not a contributor). we should have a conversation about those on the list. We need to prioritize.
</p>
<h4><span class="mw-headline" id="TOPIC:_TPAC">TOPIC: TPAC</span></h4>
<p>TPAC is W3C's annual "all hands" face-to-face meeting. Where we gather (almost) all the groups in a big conference. This year it is in Shenzhen, China. Renoir, Doug and Eliott will be there. Doug and Renoir be there between 11/9-17. Eliott: 11/10-16.
</p><p>Renoir will be going around and learn with various working groups.  Granted to be on an offset time zone and will be there for emergencies and things that have to be done.
</p><p>Renoir will also be organizing TPAC's "Lightnening talks" sub-event.
</p><p>Doug will be presenting with Eliot about WPD at TPAC to raise awareness.
</p><p>Doug is part of many working groups, and so will have limited availability.
</p><p>Doug &amp; Renoir will not be available for the next 2 General meetings, so Doug will provide Julee with status before the general meetings, so they can continue as needed.
</p><p>ACTION: While at TPAC, Doug will convey status on all pending projects before Friday General Meetings.
</p>
<h4><span class="mw-headline" id="TOPIC:_Migration">TOPIC: Migration</span></h4>
<p>Renoir has done a plan. <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Infrastructure/analysis/2013-Migrating_to_a_new_cloud_provider">http://docs.webplatform.org/wiki/WPD:Infrastructure/analysis/2013-Migrating_to_a_new_cloud_provider</a>
</p><p>The HP contract is over. Doug is going to ask HP for another extension &amp; offer HP visibility (find better word later) on the fact they started the project with us
</p><p>Dreamhost is enthusiastic to host for free our full environment, but their new system is not ready for us. They will provide a full (vanilla) OpenStack environment. They are providing us a Replication MySQL node to help the migration and testing. As soon as the OpS installation is ready, Renoir set up the full migration work.
</p><p>The time line depends upon Dreamhost to provide the environment (a blocker). Once we have in control immediately, Renoir thinks it should take a few days, then testing, as described in the doc. But the time he can't say, a lot of search &amp; replace, and then the test, and then the live db transfer is the longest time.
</p><p>Renoir says he's ready, just waiting. Doug says Renoir already started the migration, that the migration is going started ASAP.
</p><p>The css properties has a dependency on a stable site. That's why we need to know when the migration work is being done.
</p><p>Renoirb wants to make it clear that we MUST have a clone of the full production/live environment as soon as possible. as when we make changes, we are working on the production and a simple mistake can impact stability, and a change should only be a run of a script been tested many times before being run on the live site.
</p><p>ACTION: Doug will contact Dream host and get dates, today.
</p>
<h4><span class="mw-headline" id="TOPIC:_Compatibility_tables">TOPIC: Compatibility tables</span></h4>
<p>Ronald Mansveld is working on the data model so all contributing sites can provide content according to the model.
</p><p>We then need to find a way to present to the users, and how mechanically to sync the data. Doug did contract <a class="external text" href="http://www.mediawiki.org/wiki/User:Aaron_Schulz">Aaron Schulz</a> to prepare an utility to cache generated data, and thinks he's close to completion. But, since we might migrate away from MW. We do not need to have this data live. We just need to refresh the data, say, once per week.
</p><p>We do not need an automated data at this time. Priority is to have the data available in a re-usable format and present within the wiki. Need to test (today) on the computability table.
</p><p>We will disable editing the compatibility section. Julee suggested previously that if users find contrary data, they could submit an update (preferably test-driven, conforming to data model) to github. This community data source will then be one of the data sources. We might also find a way to plug to TestTheWebForward data.
</p><p>Eliot request a mechanism to report an error or flag.
</p><p>Phase one, however, is just to get some data into the css pages so we can get the css properties project out. We want to use MDN data first, and maybe caniuse.
</p><p>Janet Swisher didn't know Ronald Mansveld was working on MDN data. If jswisher had known, she could have connected him with the right folks, she'll try and do so in the future. (jswisher confirmed that ronaldmasveld did talk to appropriate people at Mozilla London)
</p><p>Doug believes we can finish Compatibility tables by the end of TPAC and possibly during it, should be at least in a working state and to test it. It would include not only the CSS properties, but be done across all features.
</p><p>ACTION: Doug will confirm dates with Ronald Mansveld &amp; Aaron Schulz today.
</p>
<h4><span class="mw-headline" id="TOPIC:_CSS_vs._Beta_announcement">TOPIC: CSS vs. Beta announcement</span></h4>
<p>For the CSS properties project, Doug suggests we "Declare victory and go home"
</p><p>There is a need for us to say thank you to the community. By mid-November, we will be in a moment where we can do so.
</p><p>But as jkomoros said, we have 1 more chance to make a big splash. So, we shouldn't call this beta.
</p><p>Questions: why have a beta? when is a good time to have a beta?
</p><p>Maybe it isn't good to announce between thanksgiving &amp; xmas. Let's give a status update and showing achievements, just announce round 1 of css properties. Then, find an appropriate time to announce a beta when we have enough "meat" to show off as we only have one shot.
</p><p>We could make a big fanfare, a coming ceremony for the beta, but we might never come to a point where we are in a complete, final state as it is the nature of the subject of the project. But we're not close to a beta announcement right now. A beta launch needs to be to the same level of efforts as the launch announcement. It might not be sufficient to only announce the css properties as the beta. The beta should include more. We should carefully consider what we have to say and what we're going to. How we are going to frame this. This round 1 of the css properties edits will be one of many granular announcements.
</p><p><br />
</p><p>We've been talking publically about CSS properties, that's what we should announce.
</p><p>Many folks agreed.
</p><p>Julee again mentioned that we need to have a timeline for the compatibility tables &amp; migration, so we know when css properties can be launched. (See discussions &amp; outstanding action items from previous meetings.)
</p><p>(On the IRC, renoirb also suggests also this as a blog post: <a rel="nofollow" class="external free" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Oct/0148.html">http://lists.w3.org/Archives/Public/public-webplatform/2013Oct/0148.html</a>)
</p>
<h4><span class="mw-headline" id="TOPIC:_Next_content_project">TOPIC: Next content project</span></h4>
<p>We need to find what we work on during DocSprint and WPW.
</p><p>JavaScript pages? 
</p><p>What is the timeframe for the JavaScript import?
</p><p>ACTION: Doug will contact Max Polk today.
</p><p>Doug thinks we already have the script to import, so should make importing easy. It might take a week or so prior to make it work.
</p><p>So, if JS is ready to import, do we want to assume that the next subject to be JavaScript?
</p><p>Doug: (thinks) that we could have room to do two subject in the same time. Doug thinks we can get a limited set of people to contribute to JavaScript, and then have a larger pool of folks who could contribute to HTML pages.
</p><p>Julee believes we do not have enough resources to manage two content projects at the same time.
</p><p>Renoirb believes his community management dashboard would help.
</p><p>ACTION: Julee to send out notes so more folks can comment on the next content project.
</p>
<h3><span class="mw-headline" id="ACTION_ITEMS">ACTION ITEMS</span></h3>
<ul><li> While at TPAC, Doug will convey status on all pending projects before Friday General Meetings.</li>
<li> Doug will contact Dream host and get dates, today.</li>
<li> Doug will confirm dates with Ronald Mansveld &amp; Aaron Schulz today.</li>
<li> Julee to send out notes so more folks can comment on the next content project.</li>
<li> Doug will contact Max Polk today.</li></ul>
<h2><span class="mw-headline" id="Agenda_2013-10-25:_Canceled_due_to_lack_of_quorum">Agenda 2013-10-25: Canceled due to lack of quorum</span></h2>
<h2><span class="mw-headline" id="Agenda_2013-10-18">Agenda 2013-10-18</span></h2>
<ul><li> CSS Properties Project</li></ul>
<table class="wikitable" style="text-align: center; width:50%">
<tr>
<th> Status
</th>
<th> Number
</th></tr>
<tr>
<td> done
</td>
<td> 257
</td></tr>
<tr>
<td> In Progress (Dave)
</td>
<td> 3
</td></tr>
<tr>
<td> Low Priority
</td>
<td> 105
</td></tr>
<tr>
<td> Needs examples (clip-rule, Doug)
</td>
<td> 1
</td></tr>
<tr>
<td> Obso/Deprec
</td>
<td> 28
</td></tr>
<tr>
<td> Vivienne just took! (table-layout)
</td>
<td> 1
</td></tr>
<tr>
<td> Grand Total
</td>
<td> 395
</td></tr></table>
<ul><li> CSS Properties Project
<ul><li> clip-rule status, Doug?</li>
<li> who will volunteer for table-layout?</li>
<li> other dependencies?
<ul><li> compatibility tables</li>
<li> legacy MSDN samples, related pages, and syntax section?</li>
<li> flag simplification?</li>
<li> review from CSS experts, spec editors &amp; rockstars?</li>
<li> launch plan?</li>
<li> should we migrate first?</li></ul></li></ul></li>
<li> migration plan</li>
<li> JS project plan
<ul><li> Should we do a plan, including community management, after a post-mortem on the CSS properties project?</li>
<li> A bulk of work gets done at Doc Sprints, should plan include proposing Doc Sprints on a regular basis to get a bunch of stuff done?</li></ul></li>
<li> WPD table at <a rel="nofollow" class="external text" href="http://html5devconf.com/">html5devconf</a> in SF: please volunteer</li>
<li> Internal Doc Sprint to get landing page &amp; other site organization cleared up?</li>
<li> Doc-Sprint-In-A-Box, Piwik reporting: this is a job for the Cracker-Jack Analytics Team!
<ul><li> A cogent set of steps for generating reports</li>
<li> What metrics shall we report?</li>
<li> Better UI for Piwik (presently unintelligible) - if possible
<ul><li> "Goals &gt; Saves a Page" path makes no sense (what is this, some kind of mangled translation?)</li>
<li> What the heck is a "conversion?"</li>
<li> (I mean, really, sometimes this open-source stuff is incorrigible!)</li></ul></li></ul></li>
<li> Doc Sprint, New York in December
<ul><li> Pro: New York, baby!</li>
<li> Con: We're not ready yet; let's get JavaScript imported and scoped first</li></ul></li></ul>
<h3><span class="mw-headline" id="Discussion_2">Discussion</span></h3>
<h4><span class="mw-headline" id="TOPIC:_CSS_Properties_Project">TOPIC: CSS Properties Project</span></h4>
<p>Last night we had one property unowned but vivienne (who was at Zurich's docsprint) took it (yay!!!) she's great, from Jay's group what we have outstanding are a few properties that Dave is working on. We're not going to do an example for knockout. We created a correct syntax example, but put a larger example on hold. All of the remainders will get live code examples at code.webplatform.org. clip-rule example, Doug is working on. We should be done mid next week (Dave is out next Wed-Fri). [much rejoicing]
</p>
<h5><span class="mw-headline" id="Subtopic:_Dependency_on_compatibility_tables">Subtopic: Dependency on compatibility tables</span></h5>
<ul><li> compatibility tables: first one is compat tables lots of activity about that this week, shepazu provided an update: at the doc sprint in amsterdam, we got to gether with PPK (he's from quirksmode, obviously) he invited the guy who does html5test.com he's been doing something like caniuse for something like ten years they're test driven what we want to do with this project is have a single data model that captures browser compat/test results for as much as we can we have permission to use MDN data, and because they are facts, we don't HAVE to attribute that use (but we plan to give attribution, just not changing the license on the articles that include it) Max Firdman (sp?) from MobileHtml5 wants to help too <a rel="nofollow" class="external free" href="http://mobilehtml5.org/">http://mobilehtml5.org/</a> <a rel="nofollow" class="external free" href="http://html5test.com/">http://html5test.com/</a> shepazu has a running prototype of a mediawiki extension that inserts compat information but it's a naive implementation and would cause caching problems html5test.com source code: <a rel="nofollow" class="external free" href="https://github.com/NielsLeenheer/html5test">https://github.com/NielsLeenheer/html5test</a> the page would be constantly changing so it wouldn't be able to be cached by CDN I'm working on another approach renoirb has good ideas on that I got renewed energy from several people a guy named Ronald Manzfeld (sp?) stepped up and said, "if you need some server-side help, I could help" he got really into the idea of making the unified data model he started on that and has a first draft available. Niels Leenheer, guy behind html5test.com PPK, NIls (HTML5Test) and others are all on a new list: public-webplatform test. Ronald has been very active, interested in driving things forward we're also going to provide an aPI so others can get it (same API we will use) I think within a couple of weeks we'll have at least something workable</li></ul>
<p>Granularity is part of the data model at docsprint, we all kind of agreed that we like the way that MDN chose a good level of granularity. there are several kinds of granularity: per feature, per browser version we thought the MDN model was pretty good, so we'll start with that. if we don't have the right kind of granularity, we'll fall back to MDN which will also be good in terms of completeness. lik ecaniuse only tests things that are new and up and coming and MobileHTML5, his granularity is quite different from caniuse. We're going to try to categorize their broader categories and capture that at a diferent level of granularity.
</p><p>public-webplatform-tests?
</p><p>ACTION: shepazu to send link to the public-webplatform-test list to main list [DONE]
</p><p><br />
We'll do batch updates once a week or so the people who are involved in this (the data sources) are likely all amendable to changing their own data models a little bit. to make it easier to integrate one exception to the updates: probably won't pull from MDN very frequently probably a one time, given that there's not as good of an API there we'll have to come up with some tests for the tests to make sure our data retrieval kept the integrity of the system. This is great, especially having so many people pitching in with experience in this area. Hoping to complete by end of november at latest. 
</p><p>Do we have a plan for if someone finds an error in the data on WPD?
The plan was to punt on that for now. Will expose our data on GitHub as well. we'll likely ask people (to start) to submit a PR wonders if we could have useful data from there <a rel="nofollow" class="external free" href="http://www.chromestatus.com/features">http://www.chromestatus.com/features</a> although of course ultimately we'll need to come up with an easy way to change it from our system probably not all that useful, but might be good for spot checking.
Could be a phased approach where for the 260 properties if we do an early import, even if it's just from one source so we could not wait too long. 
ACTION: shepazu Talk to Ronald about perhaps doing a phased compat table approach, where we just do one data source to start (in order to move faster)
</p><p>what does a conteingency plan look like? if we run into problems with the extension I'm writing (I'm going to talk to trenoirb and ryanlane later today about that, by the way) one possible contingency is to make a script to use the API for MDN to pull out their compat information, and we write a script to inserts that compat information into our pages. not generate a new page, just edit the apges we have make sure it's not automatically generated at serve time. Even if it's not possible to fully automate, even if we can automate the hard parts, we might be able to make it feasible for a small number of volunteers to copy/paste/massage my point is mainly "just think scrappy" If full-automatic isn't easy, even semi-automatic is better than nothing.
</p>
<h5><span class="mw-headline" id="Subtopic:_Dependency_on_legacy_MDN_samples">Subtopic: Dependency on legacy MDN samples</span></h5>
<p>Some residual sections were imported (especially code examples, related pages and syntax) automatically. we had talked with renoirb about doing a bulk find/replace operation if we can't do it by script, we can probably do it manually--just need some volunteers
Eliot: We're hoping to get confirmation today for a facilities reservation for University of Washington on 11/2 that sounds like a great project for students to tackle.
[murmurs of agreement]
if renoirb can run a script to at least identify pages that need this, that would be helpful, but he has a lot to tackle right now I have a lot of other things on my plate
scottrowe_: There's a lot on renoirb's plate, we should have a separate meeting to figure out prioritzation of infrastructure tassks
renoirb: For now my focus is on migration
ACTION: julee to write up bug (cc eliot) about investigating feasibility of finding pages that need old MSDN sections removed
</p>
<h5><span class="mw-headline" id="Subtopic:_Dependency_on_reviews_by_experts">Subtopic: Dependency on reviews by experts</span></h5>
<p>Review by experts &amp; get them thinking about the project so they're ready to talk about the launch when it happens. Two categories: spec experts, and rockstars the former is for shepazu, the latter is for jkomoros
ACTION: jkomoros to ask paul_irish to do a spot check of WPD CSS properties
</p>
<h5><span class="mw-headline" id="Subtopic:_Dependency_on_launch_plan">Subtopic: Dependency on launch plan</span></h5>
<p>jkomoros on that AI basic idea is a plan for a few weeks from now about blog post, who to get to support the launch.
ACTION: jkomoros to create strawman launch plan (including relative timeline)
What's the timeline?
The long pole is the compat tables for now so that will depend on information from that taskforce about if they can do a quick and dirty import.
So we're going to say we're dependent on that functionality, it's a good idea to have compat information, even if it's not the Super Awesome Amazing Automatic version
We might have a contingency plan for CSS properties, even if the SAAA version isn't ready yet so let's get feedback from compat table group, and base dates on that.
</p>
<h5><span class="mw-headline" id="Subtopic:_Dependency_on_migration">Subtopic: Dependency on migration</span></h5>
<p>Doug earlier brought up: should we migrate before announcing? But says
"no." The new provider is getting prepped to beta, a feature we could use at the end of the month I told renoirb to consider migration as top priority. Ideally ryan can help with it as well
[09:41:14] Ryan_Lane nods
[09:41:14] &lt;Ryan_Lane&gt; I can
Since we're blocked on compat tables, at least starting the migration could be a good thing.
One question is: if we finish before migration, do we wait for migration/ slash, is there enough bandwidth to do compat tables and migration? renoirb will advise on compat tables, but the two work streams don't overlap TOO much but I'll verify with Ronald
ACTION: shepazu to verify with Ronald/renoirb that compat tables and migration work streams are independent.
</p><p>Renoirb has a branch where I got less-and-less hardcoded configuration. Which is the main requirement to migrate. We can almost definitely do it without downtime.
</p><p>The other question is the risk of the migration: Whether it will cause more problems. We're not not sure. We have a known "OK-not-great" solution now. The new solution is an unknown. We should COUNT on errors during migration. 
No matter what, after a migration we'd need to test. We have a hard stop with current provider so we need to work back from that key date. It would be nice to see what that timeline looks like--a couple of days, a couple of years--then we can map that against a timeline for releasing CSS properties project if we find that things like "announcing" are overlapping with "testing", it won't be good.
ACTION: shepazu to confirm date of contract expiration with current hosting provider
ACTION: julee to make basic timeline for completing CSS prop project;
ACTION: renorib to create basic timeline on migration
</p><p>Then, we can see how they interact.
</p>
<h4><span class="mw-headline" id="TOPIC:_JS_project_plan">TOPIC: JS project plan</span></h4>
<p>We could do a postmortem on CSS props project (even in email), figure out what worked and what didn't. Use that to inform a high-level plan of tackling JS project
Doc Sprints lead to TONS of work getting done so JS project plan should incorporate a schedule of doc sprints that different folks could volunteer to run.
About.com who is enthusiastic about JS topic in particular for their upcoming doc sprint.
JS plan should be ready by December. During November, we should prep for this.
ACTION: shepazue to work with Max Polk to make sure his migration is up to speed we got review from two different experts on the JS architecture
ACTION: shepazu to forward e-mails from JS experts about architecture on to list ideally we'd run through a few WPW sprints before the doc sprint to make sure we're ready for the doc sprint
WPW is an ongoing second tier to in person doc sprints so we should pay attention to that during planning.
</p>
<h4><span class="mw-headline" id="TOPIC:_WPD_table_at_HTML5DevConf">TOPIC: WPD table at HTML5DevConf</span></h4>
<p>Shepazu got a table for W3C at the HTML5DevConf in SF next week we have me, Rebecca Hauk manning table but we need more volunteers we have some shirts and stickers, but we could use more swag. Shepazu has 3 free tickets for volunteers.
We left a big pile of t-shirts in Amsertdam
</p>
<h4><span class="mw-headline" id="TOPIC:_PiWik_reports_for_Doc_Sprints">TOPIC: PiWik reports for Doc Sprints</span></h4>
<p>scottrowe_ looked into generating the PiWik reports about doc sprint played around for awhile, but there's no way to scale this. We need to make some decsiions about what reports we're going to generate and provide steps for doc sprint owners and fix some things about piwik user interface but we should defer to analytics meeting. 
</p>
<h4><span class="mw-headline" id="TOPIC:_Google_contractor.21">TOPIC: Google contractor!</span></h4>
<p>Alex will let us know if Google adds another contractor. Stay tuned…
</p>
<h3><span class="mw-headline" id="Action_Items_2">Action Items</span></h3>
<ul><li> shepazu to send link to the public-webplatform-test list to main list [DONE]</li>
<li> shepazu Talk to Ronald about perhaps doing a phased compat table approach, where we just do one data source to start (in order to move faster)</li>
<li> julee to write up bug (cc eliot) about investigating feasibility of finding pages that need old MSDN sections removed</li>
<li> jkomoros to ask paul_irish to do a spot check of WPD CSS properties</li>
<li> jkomoros to create strawman launch plan (including relative timeline)</li>
<li> shepazu to verify with Ronald/renoirb that compat tables and migration work streams are independent.</li>
<li> shepazu to confirm date of contract expiration with current hosting provider</li>
<li> julee to make basic timeline for completing CSS prop project;</li>
<li> renorib to create basic timeline on migration</li>
<li> shepazu to work with Max Polk to make sure his migration is up to speed we got review from two different experts on the JS architecture</li>
<li> shepazu to forward e-mails from JS experts about architecture on to list ideally we'd run through a few WPW sprints before the doc sprint to make sure we're ready for the doc sprint</li></ul>
<h2><span class="mw-headline" id="Agenda_2013-10-11:_Canceled_due_to_lack_of_quorum">Agenda 2013-10-11: Canceled due to lack of quorum</span></h2>
<h2><span class="mw-headline" id="Agenda_2013-10-04">Agenda 2013-10-04</span></h2>
<h3><span class="mw-headline" id="Agenda">Agenda</span></h3>
<ul><li> CSS Properties status</li></ul>
<table class="wikitable" style="text-align: center; width:50%">
<tr>
<th>Status
</th>
<th>Number
</th></tr>
<tr>
<td> done
</td>
<td> 209
</td></tr>
<tr>
<td> In Progress
</td>
<td> 20
</td></tr>
<tr>
<td> Low Priority
</td>
<td> 113
</td></tr>
<tr>
<td> Needs Review
</td>
<td> 37
</td></tr>
<tr>
<td> Obso/Deprec
</td>
<td> 8
</td></tr>
<tr>
<td> TBD
</td>
<td> 60
</td></tr>
<tr>
<td> Grand Total
</td>
<td> 447
</td></tr></table>
<ul><li> site stability</li>
<li> Doc Sprint in a Box</li>
<li> WPD Birthday next Tue: list activities/URLs</li>
<li> Change this meeting time/day?</li>
<li> Anything else?</li></ul>
<h4><span class="mw-headline" id="Topic:_CSS_property_status">Topic: CSS property status</span></h4>
<p>scottrowe_ emailed the list of 95 properties
… the coordinators should contact those people individually
… and if we can't get those people, we'll reassign them
<a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Community/Meetings/General">http://docs.webplatform.org/wiki/WPD:Community/Meetings/General</a>
while scott compiled the list of properties, Julee reconstructed a master list &amp; categorized them according to status. She will put this in a google doc to manipulate it more easily
we should still have TBDs on the wiki, so people can sign up… and it's out of date
</p><p>there are about 60 that need to be done, and 35 need review
</p>
<h4><span class="mw-headline" id="Topic:_Doing_experimental_properties">Topic: Doing experimental properties</span></h4>
<p>some have said we should only work on things that are not experimental, but there's value for us to do more cutting-edge stuff since we're closer to the development of the specs and implementations
also good for SEO
we need to be careful about updating examples
The idea we had in mind is a mechanism. Isn't going to happen in the next 6 months
for now maybe we could do this: W3C has a DB, with a unique URL for each spec, so we could come up with something where we are working off a draft version , script that trolls publications every day, sends an email w/ a list of specs that have changed, validated against URL
ACTION: shepazu &amp; eliot to brainstorm w/ Robin at TPAC
</p>
<h4><span class="mw-headline" id="TOPIC:_site_stability">TOPIC: site stability</span></h4>
<p>Getting server &amp; client-side errors on dabblet
Are we doing any stability testing?
ACTION: Renoir to write up his testing plan, and add all relevant systems to that plan, such as Dabblet instance
julee: we could also ask the community to help with testing
</p>
<h4><span class="mw-headline" id="Topic:_Doc_Sprint_in_a_Box">Topic: Doc Sprint in a Box</span></h4>
<p><a rel="nofollow" class="external free" href="https://docs.google.com/document/d/1fIDssDZln2Z_DrnKliT1ymZpn_OTqdYA7rVgMaTsSk4/edit">https://docs.google.com/document/d/1fIDssDZln2Z_DrnKliT1ymZpn_OTqdYA7rVgMaTsSk4/edit</a>
ACTION: Millo to review doc sprint in a box, add some comments, and update it based on what we've learned internally
</p><p>ACTION: scottrowe do an edit pass stripped down to its main purpose which is to have community members throw doc sprint
ACTION: scottrowe to share with Patrick D'Souza for review
</p>
<h4><span class="mw-headline" id="Topic:_WPD_Birthday_next_Tue:_list_activities.2FURLs">Topic: WPD Birthday next Tue: list activities/URLs</span></h4>
<p>doing it on OCtober 8 would be best, since it's the birthday, but we have no volunteers; maybe the WPD twitter account could be the lead, and eveyone else could retweet
</p><p>scottrowe_ needs anecdotes, but I'll write the blog post
ACTION: Julee to forward Scott's email &amp; get them to commit to tweet &amp; point to the blog post. We looked very much on the same page 1 yr ago: we should look that way now.
ACTION: scottrowe_ will write the blog post, hopefully by Thursday.
</p>
<h4><span class="mw-headline" id="topic:_Change_this_meeting_time.2Fday.3F">topic: Change this meeting time/day?</span></h4>
<p>ACTION: Julee to send a query email &amp; ask if we should Change this meeting time/day?
</p>
<h3><span class="mw-headline" id="Action_Items_3">Action Items</span></h3>
<ul><li> shepazu &amp; eliot to brainstorm w/ Robin at TPAC</li>
<li> Renoir to write up his testing plan, and add all relevant systems to that plan, such as Dabblet instance</li>
<li> Millo to review doc sprint in a box, add some comments, and update it based on what we've learned internally</li>
<li> scottrowe do an edit pass stripped down to its main purpose which is to have community members throw doc sprint</li>
<li> scottrowe to share with Patrick D'Souza for review</li>
<li> Julee to forward Scott's email &amp; get them to commit to tweet &amp; point to the blog post. We looked very much on the same page 1 yr ago: we should look that way now.</li>
<li> scottrowe_ will write the blog post, hopefully by Thursday.</li>
<li> Julee to send a query email &amp; ask if we should Change this meeting time/day?</li></ul>
<p><br />
</p><p><br />
</p>
<h2><span class="mw-headline" id="Agenda_2013-09-27">Agenda 2013-09-27</span></h2>
<h3><span class="mw-headline" id="Agenda_2">Agenda</span></h3>
<ul><li> Piwik and the Analytics is back on track!
<ul><li> Analytics: Create a secret starting page that will help track activity during a doc sprint (TBD, probably next week)</li>
<li> Analytics: Improve the goal tracking using Piwik's API and JavaScript</li>
<li> Infra: Changing datacenter?</li></ul></li>
<li>  Doc-Sprint-In-A-Boxathon scheduled for next wednesday.
<ul><li> Everyone is welcome to join, Patrick.</li>
<li> Scott will send out a note.</li>
<li> Goal is to have this done before the Amsterdam Doc Sprint, possibly even earlier.</li></ul></li>
<li> CSS properties tables</li></ul>
<h3><span class="mw-headline" id="Discussion_3">Discussion</span></h3>
<h4><span class="mw-headline" id="TOPIC:_PiWik.2F_Analytics">TOPIC:  PiWik/ Analytics</span></h4>
<p>Piwik and the Analytics are back on track. Two weeks ago Renoir deployed PiWik in a different way than before without going too deep, it was in the same way as before (Fastly), putting a different tracking code on all of the pages should have covered all of the pages, with the help of Patrick, create goals in the dashboard &amp; campaigns. Now forwarding all of the e-mails to the analytics mailing list.
Julee &amp; Eliot filed a bug and I responded to an earlier filed one that represents requirements for the dashboard. At the analytics meeting next week we could consolidate requirements and finalize that list. All bugs &amp; discussion is on <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Requirements/Analytics">http://docs.webplatform.org/wiki/WPD:Requirements/Analytics</a>
Renoirb gives a rough geolocation, might need to recrunch the database; some other work: a way to trigger conversions in the goals (like clicking on edit or save), will require adding JS if we get it in place before the docsprint, we can track progress. Scott_rowe will show up at next analytics meeting to discuss.
</p>
<ul><li> ACTION: Scott_rowe to attend analytics meeting on Monday 4pm pdt</li></ul>
<h4><span class="mw-headline" id="TOPIC:_Infra:_Changing_datacenter.3F">TOPIC:  Infra: Changing datacenter?</span></h4>
<p>No news. Worked with Doug on that. Didn't get any feedback from anyone yet, but time is passing working to rebuild the VM from scratch as much as renoir can in the same environment.
We either need to move soon, or do the move next month
Still trying to connect up with Dreamhost and other folks
</p>
<h4><span class="mw-headline" id="TOPIC:_Doc-Sprint-In-A-Boxathon_scheduled_for_next_wednesday">TOPIC:  Doc-Sprint-In-A-Boxathon scheduled for next wednesday</span></h4>
<p>I asked Jay to take leadership of kicking this off I think that he is working on the general structure of the thing right now, Jay sent an e-mail about the timing, but also an e-mail from Scott and Peter where they had a draft docsprint in a box: a brain dump about all of the things we thought should be in there. Not intended to dictate the structure. just making sure that before the meeting we wrote down what we had learned from doing a few. Jay also had an idea of the structure he wanted.
</p>
<ul><li> ACTION: scottrowe to send an e-mail to the list to invite anyone who's interested to get involved with the docsprint in a box I think Jay sent an invite to Patrick, but we should confirm</li></ul>
<h4><span class="mw-headline" id="TOPIC:_CSS_properties_tables">TOPIC:  CSS properties tables</span></h4>
<p>We discussed how to manage the tables. Also, coordinators need to verify that each property they are coordinator for is properly reflected in table. Julee &amp; Eliot have done this. Chris Mills, Shepazu &amp; Nic d'Costa needs to do this. 
</p>
<ul><li> ACTION: Julee to remind Nic &amp; Doug to update their properties in the tables. [DONE]</li>
<li> ACTION:&#160;??? to contact Chris.</li></ul>
<p>We discussed doing a script to import all properties into project.webplatform.org, but really the work is manual checking at this point.
<a rel="nofollow" class="external free" href="https://scraperwiki.com/">https://scraperwiki.com/</a>
</p><p>Creating a JS project in the project tracker and populating it makes sense for when we start a new project, especially since we've fixed the sendmail time-out bug.
</p>
<ul><li> ACTION: scottrowe_ and julee to work at creating a new list of unfinished CSS properties</li></ul>
<h3><span class="mw-headline" id="Action_Items_4">Action Items</span></h3>
<ul><li> Scott_rowe to attend analytics meeting on Monday 4pm pdt [STATUS: Everyone was a no-show. Will happen next Monday, instead.]</li>
<li> scottrowe to send an e-mail to the list to invite anyone who's interested to get involved with the docsprint in a box I think Jay sent an invite to Patrick, but we should confirm  [DONE]</li>
<li> Julee to remind Nic &amp; Doug to update their properties in the tables. [DONE - Julee &amp; scottrowe did them]</li>
<li>&#160;??? to contact Chris. [Resolved]</li>
<li> scottrowe_ and julee to work at creating a new list of unfinished CSS properties  [DONE]</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="Agenda_2013-09-20">Agenda 2013-09-20</span></h2>
<p>Objective: Describe the current state of the project.
</p><p>Note, the objective does not include making any decisions or otherwise taking any actions other than those required to understand the state of the project. This should be a very short, concise meeting.
</p>
<ul><li> WPW update - status?
<ul><li> Have coordinators verified the status of each page in their purview?</li>
<li> We need to consolidate the tables into a final master list of properties to be worked on, and we want to include only those properties still being worked.</li></ul></li>
<li> WPW reinvigoration - what do we need to do to put some life back into this?
<ul><li> We've dropped to 50 active users/month.</li>
<li> Are site performance problems a contributing factor?</li></ul></li>
<li> State of WPD for the birthday - what have we accomplished?</li>
<li> Who's in for Amsterdam?</li>
<li> Doc Sprint New York?</li>
<li> We're out: print up some new t-shirts?</li>
<li> Reminder: Doc Sprint in a Box, Oct. 2</li>
<li> JavaScript import status?</li>
<li> Compatibility automation status?</li>
<li> Analytics &amp; reporting?</li>
<li> Back-end update from Renoir?
<ul><li> Piwik enhancements in a nutshell</li>
<li> Site performance - what are the problems and what is preventing solutions?</li></ul></li>
<li> Next week's blog post author</li>
<li> Anything else?</li></ul>
<h2><span class="mw-headline" id="Agenda_2013-08-23">Agenda 2013-08-23</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> <a href="/wiki/Meta:web_platform_wednesday" title="Meta:web platform wednesday">WPW</a> - how is it going?
<ul><li> <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Aug/0146.html">Additional properties to add to this project?</a></li></ul></li>
<li> Anything blocking you from creating great content?</li>
<li> Anything new &amp; notable? (Blogs or other communications planned for next week?)</li></ul>
<h2><span class="mw-headline" id="Agenda_2013-08-16">Agenda 2013-08-16</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> <a href="/wiki/Meta:web_platform_wednesday" title="Meta:web platform wednesday">WPW</a> - how is it going?
<ul><li> Schedule</li>
<li> Who's coordinating?</li>
<li> Action items cleanup: Please search for your name on this page.</li></ul></li>
<li> Infrastructure meetings</li>
<li> Communications plan</li>
<li> Anything blocking you from creating great content?</li>
<li> Anything new &amp; notable? (Blogs or other communications planned for next week?)</li></ul>
<h3><span class="mw-headline" id="Discussion_4">Discussion</span></h3>
<h4><span class="mw-headline" id="TOPIC:_WPW_-_how_is_it_going.3F">TOPIC: WPW - how is it going?</span></h4>
<p>julee: We have three coordinators, but no contributors. A lot of people are busy or on vacation. Originally we had an optimistic schedule to be done by august  after reviewing with a few folks, everyone thought that was way too optimistic  especially given summer vacation period. We will put in a buffer week after labor day, &amp; add incomplete properties back onto the pile.
After the end of august, Microsoft will have some resources that we'll be adding to this  one of my writers will be helping, another writer who hasn't worked on this yet will be helping as well.
Google is working on a contractor as well, and scottrowe will be helping out with coordinating as well
</p><p>Bumping up the boolean values for things like animated values in the CSS properties template, and also Inherited field. Maybe Frozenice can&#160;?
ACTION: julee to reach out to frozenice assigning the "non-boolean properties for animatable, etc" template issue to him
</p>
<h4><span class="mw-headline" id="TOPIC:_Servers">TOPIC:  Servers</span></h4>
<p>shepazu: We'll be talking to dreamhost later  but ryan and renoirb think it's a good thing to have redundancy across hosts  renoir contacted a few different hosts including Digital Ocean and iWeb  the latter is based in Quebec  so renoirb can talk to them in 
shepazu: Dreamhost asctually wants to be involved in the project as a steward
&lt;patrickdsouza1&gt; renoirb: good to look at hosts in a different time zone like europe.
&lt;renoirb&gt; iWeb data center: <a rel="nofollow" class="external free" href="http://iweb.com/green-data-centers">http://iweb.com/green-data-centers</a>
renoirb: I talked to them. The idea is a main one and another one that's latent, that we have a copy of everything; if we need to change we just flip a switch. Looked around for one with a good reptuation with multi site. iWeb's president is going to talk to us by Tuesday of next week
We need to have a different company/place to back up stuff on a regular basis, but if you have multiple instances across diffferent companies, you have a huge latency issue. Ryan_Lane has a preference towards openstack clouds, as its open source nature aligns well with our project  if dreamhost can provide us with the different locations/datacenters, then is the secondary company just a single backup instance? We will roll out redundancy as needed  the idea is to have redundancy between prod and test. Julee asked for an architecture document that describes our setup with a nice diagram, and references to justifing it.  
</p>
<h4><span class="mw-headline" id="TOPIC:_Server_status">TOPIC: Server status</span></h4>
<p>Also, server status page (going to be on our own sub-domain for sure): <a rel="nofollow" class="external free" href="http://webplatform.tumblr.com/">http://webplatform.tumblr.com/</a>
</p>
<h4><span class="mw-headline" id="TOPIC:_Infrastructure_meeting">TOPIC: Infrastructure meeting</span></h4>
<p>At infrastructure meeting, most of the discussion was about how to prioritize renoirb's work schedule; we're going to use projects.webplatform.org. 
Once community has a decision, having execution focused meetings is helpful to add it into the issue tracker  (if there are issues that aren't recorded yet, we'll raise them there), executing on things that have already been decided in the community meetings or over e-mail on the list, taking the decisions from the group and parsing down into actionable things and track them in project.wwebplatofm.orgexposing it in the dashboards/reports, so the current health is viewable by anyone. Everyone is welcome at the infrastructure meeting, but because julee/shepazue/renoirb are full-time on this project, we'll take responsibility to keep track. 11am Pacific on Mondays, and we can move it if others want to attend regularly.
</p><p><br />
</p>
<h4><span class="mw-headline" id="TOPIC:_Communications_plan">TOPIC: Communications plan</span></h4>
<p>There's been so much activity, I want to have people talk about what they're doing
Renoirb got access to the social medial outlets, G+, twitter, FaceBook. Ideally we'd be able to automate publishing a post to all outlets, with a buffer system to space out updates too and space out updates on different channels. Updates should be scheduled to not only USA time but for those in Europe and the rest of the world  and the status tumblr, when something happens that we want to talk about, the conversation wil lgo to the tumblr status  regarding the policies, I think we should keep it the same: vendor neutral, information on status
eliots blog proposal&#160;: how &amp; why we blog; we'll have an editorial calendar; start looking for repeating blog posts;
&lt;nicdaCosta&gt; with regards to tumblr and the new G+ community, is it necessary to have so many outlets? And would there be a given "purpose" for each outlet?
WPD calendar in g+ may not be sufficient for an editorial calendar
</p><p>looking forward to seeing Coalie Mercier, from the W3C MarComm staff, her work &amp; what she wants to do for the future
we need a regular voice
AI: R/S/J in project.wp.org, we could rename project community management; create tasks, give ownership, tag twitter, blogpost, whatever, infographics, etc.
</p>
<h3><span class="mw-headline" id="Action_Items_5">Action Items</span></h3>
<ul><li> CARRIED FORWARD: Everyone to review the general meeting notes for actions assigned to them that aren't marked "(DONE)" and update with status as described above. (Mostly done: Doug &amp; Renoir to do.) (CARRY FORWARD)</li>
<li> CARRIED FORWARD: shepazu make "can you tell if this page is ready for consumption or needs more work" an active question for css project reviewers. (CARRY FORWARD)</li>
<li> CARRIED FORWARD: Julee make sure editing guide is updated with new flag values, when flags are done. (Has a dependency on flags being done) (CARRY FORWARD)</li>
<li> CARRIED FORWARD: Alex to talk to Paul irish &amp; other folks on the list that Eliot pointed him to (a list that we created at launch?) about reviewing "done" pages. (In progress: jkomoros talked to paulirish yesterday, who is in when needed; dependency on more content being done. Tracking this in the CSS Properties endgame schedule.)</li>
<li> CARRIED FORWARD: shepazu to figure out how to move current flags to new flag types and cc jkomoros and frozenice. (CARRY FORWARD Tracking this in the CSS Properties endgame schedule.)</li>
<li> shepazu to make sure Lea incorporated Chris Coyier's feeedback as appropriate.</li>
<li> CARRY FORWARD: Shepazu &amp; renoirb to review Lea's actions item and reassign and to reassign ownership of project.webplatform.org. (CARRIED FORWARD)</li>
<li> R/S/J in project.wp.org, we could rename project community management; create tasks, give ownership, tag twitter, blogpost, whatever, infographics, etc.</li></ul>
<h2><span class="mw-headline" id="Agenda_2013-08-09_Meeting_canceled_due_to_lack_of_agenda">Agenda 2013-08-09 Meeting canceled due to lack of agenda</span></h2>
<h2><span class="mw-headline" id="Agenda_2013-08-02">Agenda 2013-08-02</span></h2>
<ul><li> Roll call</li>
<li> Welcome to Renoir!</li>
<li> Review of open action items</li>
<li> <a href="/wiki/Meta:web_platform_wednesday" title="Meta:web platform wednesday">WPW</a> - how is it going?
<ul><li> Endgame schedule</li>
<li> We need coordinators &amp; contributors -- but especially coordinators</li>
<li> Action items cleanup: Please search for your name on this page.
<ul><li> It's probably associated with an action item. Either:
<ul><li> Mark it as (DONE)</li>
<li> Mark it as (DUE: &lt;date&gt;) (really, only pre-launch or post-launch)</li>
<li> Mark it as (STATUS: NO LONGER IMPORTANT) or some other STATUS</li></ul></li>
<li> Next week, Julee will email you, and cc list, all Action items that need to be done before launch.</li></ul></li></ul></li>
<li> Analytics meeting is moving to Monday 4pmPDT/7pmEDT</li>
<li> We're going to move to proactive notification regarding system issues:
<ul><li> We'll set up a status page of server</li>
<li> We'll email public list and update the irc channel status (webplatform webplatform-site) when there's problems; when work on the system affects UX.</li></ul></li>
<li> Max's <a href="/wiki/WPD:Projects/javascript" title="WPD:Projects/javascript">JS file import plan</a> ready for language expert reviews</li>
<li> <a rel="nofollow" class="external text" href="https://www.google.com/calendar/embed?src=gqaik6l023aodhh4m24qapctpg%40group">Group calendar</a></li>
<li> SSL Certificate for TLD and sub-domains</li>
<li> Dev backlog in a new Wiki namespace; e.g. WPD:Development/ProjectA</li></ul>
<h3><span class="mw-headline" id="Discussion_5">Discussion</span></h3>
<h4><span class="mw-headline" id="TOPIC:_Welcome_to_Renoir.21">TOPIC: Welcome to Renoir!</span></h4>
<p>[much rejoicing]
</p><p>Shepazu chose Renoir because he has a good balance of backend/sysadmin skills, frontend/backend development, design, and also because of his interest in the topic and history of community outreach. Great combination of skills for this project.
</p><p>Renoir is based in Montreal, so on east coast time-zone, which is convenient for working with Shepazu but also he can be up early enough to work with europeans, but also people on the West Coast.
</p><p>We'll keep contracting with Ryan as we need him, given his expertise. Renoir has already helped with the recent instability problem.
</p><p>Official start date was August 1. Vacation to Paris for one week, August 30th
</p>
<h4><span class="mw-headline" id="TOPIC:_Lea_is_not_at_W3C">TOPIC: Lea is not at W3C</span></h4>
<p>Wednesday was Lea's last day at W3C. Lea had a great mix of design/front end skills. Renoir has some of those skills (mostly on development side). She didn't design icons, illustrations, etc, so as I'm looking for a new person we can focus on people with strong UX/UI skills, ooking at 10-12 candidates already. We have a job description on W3C's site. <a rel="nofollow" class="external free" href="http://www.w3.org/Consortium/Recruitment/#design-webplatform">http://www.w3.org/Consortium/Recruitment/#design-webplatform</a>
</p><p><br />
ACTION ITEM: julee: We need someone to review Lea's actions item and reassign, and to reassign ownership of project.webplatform.org.
</p>
<h4><span class="mw-headline" id="TOPIC:_Action_items_cleanup">TOPIC: Action items cleanup</span></h4>
<ul><li> Action items cleanup: Please search for your name on this page.
<ul><li> It's probably associated with an action item. Either:</li>
<li> Mark it as (DONE)</li>
<li> Mark it as (DUE: &lt;date&gt;) (really, only pre-launch or post-launch)</li>
<li> Mark it as (STATUS: NO LONGER IMPORTANT) or some other STATUS</li>
<li> Next week, Julee will email you, and cc list, all Action items that need to be done before launch.</li></ul></li></ul>
<p>ACTION: Everyone to review the general meeting notes for actions assigned to them that aren't marked "(DONE)".
</p>
<h4><span class="mw-headline" id="TOPIC:_WPW_-_how_is_it_going.3F_2">TOPIC: WPW - how is it going?</span></h4>
<h4><span class="mw-headline" id="SUBTOPIC:_Endgame_schedule">SUBTOPIC: Endgame schedule</span></h4>
<p>Non-content portion of the plan is probably doable. Need to confirm the compatibility table work. 
</p><p><br />
The Content part of the schedule is still at risk because of resources. Especially folks who can coordinate.
</p><p>We have 66 properties that need to be edited and also a review. It's not a huge number and something we can shoot for. We should popularize that number.
</p><p>We have a good pool of contributors, we need people who have expertise to get them on board.
</p><p>We need at least 4 coordinators for each week for next four weeks. There's shepazu &amp; julee – who have a lot of other things to do. Shepazu suggested renoirb. If renoirb and Shepazu work on coordinating the community and content, those resources will be pulled off devops, tech support, and system readiness.
</p><p>We have asked folks like nicdaCosta to coordinate. That works fine, but these volunteers are hard to come by and limited in their time.
</p><p>Should we extend the project out and give ourselves a more sane cushion, like, into September?
</p><p>Maybe if Doug/Eliot/Alex responded to stewards list, that would give more momentum.
</p><p>We need to articulate the specific, scoped work, with realistic time commitment, that might help.
</p><p>ACTION: shepazu and julie to make a more concrete plan with nubmers about steward asks, and eliot/alex will respond with their donations. [Eliot DONE]
</p><p>ACTION: shepazu to reach out to other stewards to make sure they respond to the concrete plan asking for help.
</p>
<h5><span class="mw-headline" id="SUBTOPIC:_Flags">SUBTOPIC: Flags</span></h5>
<p>Lea &amp; shepazu have the action item to actively ask reviewers:
</p><p>"can you tell if this page is ready for consumption or needs more work" 
</p><p>Basically, the requirement that when a person lands--we have 4500 pages on WPD, we've been working on 200-300. Users need to figure out when they're looking at an article, whether it's ready to consume or not.
</p><p>So flags will be moved to a more discrete place.
</p><p>Lea has prototyped the flags. renoirb has extracted those, we're ready to put them in when we get the flag stuff done.
</p>
<h4><span class="mw-headline" id="TOPIC:_dreamhost">TOPIC: dreamhost</span></h4>
<p>Shepazu talked to dreamhost (at least one person there) at hosting the site. And possibly being an active steward. 
</p><p>ACTION: renoirb: needs to be involved in the dreamhost conversations to make sure they have what we need.
</p><p><br />
</p>
<h4><span class="mw-headline" id="TOPIC:_Analytics_meeting_moving_to_Mondays">TOPIC: Analytics meeting moving to Mondays</span></h4>
<p>Analytics meeting is moving to Monday 4pmPDT / 7pmEDT.
</p><p><br />
</p>
<h4><span class="mw-headline" id="TOPIC:_Max.27s_JS_file_import_plan">TOPIC: Max's JS file import plan</span></h4>
<p>Max's JS file import plan ready for language expert reviews
<a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Projects/javascript">http://docs.webplatform.org/wiki/WPD:Projects/javascript</a>
</p>
<h4><span class="mw-headline" id="TOPIC:_Google_Calendar">TOPIC: Google Calendar</span></h4>
<p>Google calendar is up. This is most presently for folks to add the times where they're available to help with WPD, and when they're unavailable.
</p><p>renoirb: can see the calendar there, no events
</p><p><br /> 
<a rel="nofollow" class="external free" href="https://www.google.com/calendar/embed?src=gqaik6l023aodhh4m24qapctpg%40group">https://www.google.com/calendar/embed?src=gqaik6l023aodhh4m24qapctpg%40group</a>
</p><p><br />
</p>
<h4><span class="mw-headline" id="TOPIC:_proactive_notification_regarding_system_issues">TOPIC: proactive notification regarding system issues</span></h4>
<p>We're going to move to proactive notification regarding system issues
</p>
<ul><li> We'll set up a status page of server</li>
<li> We'll email public list and update the irc channel status (webplatform webplatform-site) when there's problems; when work on the system affects UX.</li></ul>
<p>Renoir set up a system that will notify himself and Doug when the site is down.
</p><p>Low-hanging fruit to set up have a simple system that lets people know what the status is if it's going wrong. Something like status.webplatform.org, to say either it's a known outage or unknown. 
</p>
<h4><span class="mw-headline" id="TOPIC:_Dev_backlog">TOPIC: Dev backlog</span></h4>
<p>Dev backlog in a new Wiki namespace; e.g. WPD:Development/ProjectA
</p><p>That way, we can store dev projects there.
</p><p>When your infra fails… it happens to also affect the status view.
</p><p>Please use project.webplatform.org when possible to create and track projects once they move from the proposals phase.
</p>
<h4><span class="mw-headline" id="TOPIC:_SSL_Certificate_for_TLD_and_sub-domains">TOPIC: SSL Certificate for TLD and sub-domains</span></h4>
<p>No time to discuss SSL Certificate for TLD and sub-domains.
</p><p>renoirb &amp; shepazu will take it off line.
</p>
<h3><span class="mw-headline" id="ACTION_ITEMS_6">ACTION ITEMS</span></h3>
<ul><li> CARRY FORWARD: Everyone to review the general meeting notes for actions assigned to them that aren't marked "(DONE)" and update with status as described above. (STATUS: Mostly done: Doug &amp; Renoir to do.) (CARRIED FORWARD)</li></ul>
<p>AI: renoirb: needs to be involved in the dreamhost conversations to make sure they have what we need. (DONE &amp; ongoing)
AI: shepazu and julee to make a more concrete plan with numbers about steward asks, and eliot/alex will respond with their donations. (DONE)
AI: shepazu to reach out to other stewards to make sure they respond to the concrete plan asking for help. (STATUS: In progress - eliot found that mail to be eloquent and effective. Tracking this in the CSS Properties endgame schedule.)
</p>
<ul><li> shepazu to look into if we need separate HTMLElement and SVGElement templates for ITS project (Unless they come to us with problems, we'll assume they're okay)</li>
<li> Jirka to create overview/tutorial on ITS. (STATUS: In progress.)</li>
<li> shepazu to confirm compatibility tables will be done in time. (STATUS: Not much progress because of renoir's other duties, we made good progress before that, it's high on Renoir's priority list, once stability stuff and reporting stuff is done, it's not going to be that much work after that. Tracking this in the CSS Properties endgame schedule.)</li>
<li> Julee to call out in property review checklist that people should verify MSDN examples, and either replace with better examples or move to code.webplatform.org. (DONE: <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/Meta:web_platform_wednesday/reviewer_checklist">http://docs.webplatform.org/wiki/Meta:web_platform_wednesday/reviewer_checklist</a>)</li>
<li> CARRY FORWARD: shepazu make "can you tell if this page is ready for consumption or needs more work" an active question for css project reviewers. (CARRIED FORWARD)</li>
<li> CARRY FORWARD: Julee make sure editing guide is updated with new flag values, when flags are done. (Has a dependency on flags being done) (CARRIED FORWARD)</li>
<li> CARRY FORWARD: shepazu to figure out how to move current flags to new flag types and cc jkomoros and frozenice. (CARRIED FORWARD Tracking this in the CSS Properties endgame schedule.)</li>
<li> CARRY FORWARD: shepazu to contact CSS wg about reviewing "done" pages. (Leaverou started a thread, but not to CSSWG. Dependency on more content being done.) (CARRIED FORWARD Tracking this in the CSS Properties endgame schedule.)</li>
<li> CARRY FORWARD: Alex to talk to Paul irish &amp; other folks on the list that Eliot pointed him to (a list that we created at launch?) about reviewing "done" pages. (STATUS: In progress: jkomoros talked to paulirish yesterday, who is in when needed; dependency on more content being done.) (CARRIED FORWARD Tracking this in the CSS Properties endgame schedule.)</li>
<li> CARRY FORWARD: Shepazu &amp; renoirb to review Lea's actions item and reassign and to reassign ownership of project.webplatform.org. (CARRIED FORWARD)</li>
<li> ACTION ITEM: Shepazu to talk to Ryan about the 503s. (DONE: Garbee and Renoir talked to him more extensively, a bunch of jobs weren't getting performed, and the backlog was causing problems. Think he's resolved that.)</li>
<li> renoir to look at server errors in more depth. (DONE: Got more confirmation last week; a hard confirmation. Working this afternoon to make the piwik switch today. Trying to recreate infrastructure locally to be able to test it. Succeeded in getting it running locally, will publish my workspace on github soon, so anyone else can build it completely after, of course, removing sensitive information and history</li>
<li> CARRY FORWARD: shepazu to reach out to Julien and Rick Byers regarding JS plan. (STATUS: In progress: Shepazu reached out to rick byers, julien, and rick Waldron. Needs to pass info back to Max.)</li></ul>
<h2><span class="mw-headline" id="Agenda_2013-07-26_Meeting_canceled_due_to_lack_of_quorum">Agenda 2013-07-26 Meeting canceled due to lack of quorum</span></h2>
<h2><span class="mw-headline" id="Agenda_2013-07-19_Meeting_canceled_due_to_lack_of_quorum">Agenda 2013-07-19 Meeting canceled due to lack of quorum</span></h2>
<h2><span class="mw-headline" id="Agenda_2013-07-12">Agenda 2013-07-12</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> ITS</li>
<li> <a href="/wiki/Meta:web_platform_wednesday" title="Meta:web platform wednesday">WPW</a> - how is it going?
<ul><li> Other MBF issues?
<ul><li> compatibility tables (Doug)</li>
<li> data types &amp; units done (Julee) (DONE)</li>
<li> code samples switched from MSDN to code.webplatform.org
<ul><li> Julee to add it as a review checklist (DONE)</li></ul></li>
<li> schedule high-level reviews (Doug &amp; Lea)
<ul><li> CSS WG, for instance: template change recommendations of WG? (e.g.: animatable is not a simple boolean)</li>
<li> visual, or UI indication of whether or not any given page is ready or not</li>
<li> incorporate Chris Coyers UI feedback (Lea)</li></ul></li>
<li> review from famous devrel people (paul irish, chris coyier) (Alex)
<ul><li> visual, or UI indication of whether or not any given page is ready or not</li></ul></li>
<li> a launch plan (Alex)</li>
<li> All systems ready check
<ul><li> We can handle additional traffic</li>
<li> All SysOps &amp; DevOps folks are notified to expect additional traffic &amp; should not tweak the site during the first</li></ul></li></ul></li>
<li> Who will be a coordinator for the next 2 weeks?</li></ul></li>
<li> Max's JS file import</li>
<li> Anything blocking you from creating great content?</li>
<li> Anything new &amp; notable? (Blogs or other communications planned for next week?)</li></ul>
<h3><span class="mw-headline" id="Discussion_6">Discussion</span></h3>
<h4><span class="mw-headline" id="Topic:_Zurich_docsprint">Topic: Zurich docsprint</span></h4>
<p>Jay asked for retweeting from various official twitter handles about the Zurich Docsprint.
</p><p>Please retweet and otherwise promote: here: <a rel="nofollow" class="external free" href="https://twitter.com/klick_ass/status/355063210086383619">https://twitter.com/klick_ass/status/355063210086383619</a>  +1/Share this:<a rel="nofollow" class="external free" href="https://plus.google.com/u/0/100575683580946332118/posts/EjJ9r6WCBXg">https://plus.google.com/u/0/100575683580946332118/posts/EjJ9r6WCBXg</a>  Repost here: <a rel="nofollow" class="external free" href="https://alpha.app.net/klick_ass/post/7550831">https://alpha.app.net/klick_ass/post/7550831</a> 
</p>
<h4><span class="mw-headline" id="Topic:_Jirka.27s_ITS_project">Topic: Jirka's ITS project</span></h4>
<p>Jirka shared with us:
</p><p>ITS developed something back 6 years ago in Firefox, mainly for XML, also XHTML just a set of metadata that could help translation like a translate attribute that could say whether or not the content should be translated. ITS developed several such attributes, and because it was not sufficient for more complex things, we developed v2.0 which added more localization metadata. because it was clear that HTML5 was taking off, we provided a way to map those attributes to they have a prefix. It's published as a proposed recommendation. Not expecting any changes to 
not all implementations make use of all ITS attributes yet. For example, Google Translate and Microsoft Translate support translate attribute. And that attribute also is now in HTML5 formally. We thought it might be a good idea to recommend those attributes on web platform.org, since they're an integral part of HTML (or becoming that way).
</p><p>Action Item: Jirka to send to the public email list something where we can see it in action? public showcases, videos, slides.
</p><p>ITS should have its own namespace on WPD. But we should consider other things about the translation or multi-lingual stuff that might be a better larger bucket, such as unicode stuff, or some other internationalization bucket, a internationalization/multi-lingual namespace…
</p><p>Reference area as well.
</p><p>ITS is mostly attributes, with a few elements. It's a little bit tricky because HTML doesn't allow you to use your own elements in own namespace. So you can interlink to an external ITS file, similar to linking a stylesheet.
</p><p>ITS probably will not require any templates than our current Element and Attribute templates.
</p>
<h4><span class="mw-headline" id="Topic:_CSS_Properties_project_end_game">Topic: CSS Properties project end game</span></h4>
<h5><span class="mw-headline" id="Subtopic:_Stuff_to_do_before_we_are_.22done.22">Subtopic: Stuff to do before we are "done"</span></h5>
<p>(See outline of things blocking us completing the project.)
</p><p>We think we can get the compatibility tables done in time.
</p><p>ACTION ITEM: shepazu to confirm compatibility tables will be done in time.
</p><p>ACTION ITEM: julee to explain on the list what's happening with the messy data types, defining what we need to do to fix it. (DONE)
</p><p>A lot of the content that was donated had samples in them. The view sample link points to MSDN. We need to switch the code samples from MSDN to code.webplatform.org.
</p><p>But really, a lot of the samples are stale. They should be reviewed.
</p><p>Easiest fix: after pages have been updated and reviewed, search for MSDN links and delete any of those links. More complex: programmatically update to move to code.webplatform.org.
</p><p>ACTION ITEM: Julee to call out in property review checklist that people should verify MSDN examples, and either replace with better examples or move to code.webplatform.org. (DONE)
</p>
<h5><span class="mw-headline" id="Subtopic:_Visual_indication_that_a_page_is_.22done.22">Subtopic: Visual indication that a page is "done"</span></h5>
<p>How can the user tell if a page is ready for consumption or not. We're working on P2-P3 properties, but there are a bunch more. Want to make it clear to users which ones are vetted. 
</p><p>Are our new flags a good enough indication to first-time visitor that it's ready for consumption? Yes, if we are  consistent. 
</p><p>ACTION ITEM: Lea &amp; shepazu make "can you tell if this page is ready for consumption or needs more work" an active question that they're asking people in the other reviews, validate with folks that it's clear with them. 
</p><p>ACTION ITEM: Julee make sure editing guide is updated with new flag values, when flags are done.
</p><p>ACTION ITEM: Lea &amp; shepazu to figure out how to move current flags to new flag types and cc jkomoros and frozenice.
</p>
<h5><span class="mw-headline" id="Subtopic:_High_level_.22expert.22_reviews">Subtopic: High level "expert" reviews</span></h5>
<p>We'd like to get feedback, fine touches, and the green light from CSS working group and other "famous devrel people".
</p><p>ACTION ITEM: shepazu to contact CSS wg about reviewing "done" pages.
ACTION ITEM: Alex to talk to Paul irish &amp; other folks on the list that Eliot pointed him to (a list that we created at launch?) about reviewing "done" pages.
</p><p>ACTION ITEM: Lea to incorporate Chris Coyier's feeedback as appropriate.
</p>
<h5><span class="mw-headline" id="Subtopic:_System_stability">Subtopic: System stability</span></h5>
<p>Julee &amp; others are getting a lot of 503 issues.
</p><p>ACTION ITEM: Shepazu to talk to Ryan about the 503s
</p><p>Maybe we need a "systems ready" line item in the guidelines for launching. If we get activity for this "launch", we should be confident we aren't going to crash.
</p><p>Also, need to let Ryan and all know not to tweak production site for first few weeks of launch.
</p><p>Also leaverou reported a bug on production site. She can't deploy to test wiki, only production wiki.
</p><p>ACTION ITEM: Lea to send infrastructure bug (can't deploy to test wiki, only production wiki) directly to Ryan. (DONE)
</p>
<h5><span class="mw-headline" id="Subtopic:_we_need_more_coordinators">Subtopic: we need more coordinators</span></h5>
<p>Julee and shepazu cannot keep up with the contributors and properties. We need coordinators. So, every Tuesday, please volunteer. Eliot is busy until August. (Props to Eliot for calling in on vacation!)
</p><p>When active folks are going to be unavailable, we need to have people hand off the things to someone else.
</p><p>Up-front work, but then we have another coordinator! 
</p><p>We had some good coordination beginning, but it's petered off. Folks are generally concurring: people are distracted with other things, it's the middle of summer…
</p><p>Julee is manually going back to previous contributors and re-engaging.
</p><p>It's fine to have this problem NOW, but to make sure it doesn't happen in the future, we need to establish a mechanism.
</p>
<h4><span class="mw-headline" id="Topic:_JS_import_project">Topic: JS import project</span></h4>
<p>Max and Phistuck have been working out the final structure of the JS import.
Let's get some JS experts who would be interested in reviewing the structure they're working out.
Also, they might be at a blocking point; relying on naming convention for DOM, which I'm not sure if we settled or not.
We need to sort out the details for the import.
</p><p>We want to make sure they're not aiming at a moving target on the DOM side.
</p><p>ACTION ITEM: shepazu to reach out to Julien and Rick Byers.
</p><p>ACTION ITEM: Julee to make sure we have one page where we solidify what Phistuck and Max want.
</p><p>ACTION ITEM: jswisher to reach out to Dave Brouant (sp?) 
</p>
<h3><span class="mw-headline" id="Action_Items_7">Action Items</span></h3>
<ul><li> shepazu to look into if we need separate HTMLElement and SVGElement templates for ITS project</li>
<li> Jirka to create overview/tutorial on ITS.</li>
<li> shepazu to confirm compatibility tables will be done in time.</li>
<li> julee to explain on the list what's happening with the messy data types, defining what we need to do to fix it. (DONE)</li>
<li> Julee to call out in property review checklist that people should verify MSDN examples, and either replace with better examples or move to code.webplatform.org. (DONE)</li>
<li> Lea &amp; shepazu make "can you tell if this page is ready for consumption or needs more work" an active question that they're asking people in the other reviews, validate with folks that it's clear with them. </li>
<li> Julee make sure editing guide is updated with new flag values, when flags are done.</li>
<li> Lea &amp; shepazu to figure out how to move current flags to new flag types and cc jkomoros and frozenice.</li>
<li> shepazu to contact CSS wg about reviewing "done" pages.</li>
<li> Alex to talk to Paul irish &amp; other folks on the list that Eliot pointed him to (a list that we created at launch?) about reviewing "done" pages.</li>
<li> Lea to incorporate Chris Coyier's feeedback as appropriate.</li>
<li> Shepazu to talk to Ryan about the 503s</li>
<li> Lea to send infrastructure bug (can't deploy to test wiki, only production wiki) directly to Ryan. (DONE)</li>
<li> julee to explain on the list what's happening with the messy data types, defining what we need to do to fix it. (DONE)</li>
<li> shepazu to reach out to Julien and Rick Byers regarding JS plan.</li>
<li> Julee to make sure we have one page where we solidify what Phistuck and Max want.(DONE)</li>
<li> jswisher to reach out to Dave Brouant (DONE) </li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="Agenda_2013-06-28">Agenda 2013-06-28</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> <a href="/wiki/Meta:web_platform_wednesday" title="Meta:web platform wednesday">WPW</a> - how is it going?
<ul><li> Who will be a coordinator for the next 4 weeks?</li>
<li> How should we circle back around to folks who have previously showed interest?
<ul><li> Julee started a CRM for community contributors. (DONE)</li></ul></li>
<li> What MBF for CSS properties?
<ul><li> compatibility tables</li>
<li> data types &amp; units done</li></ul></li></ul></li>
<li> Demian's Tech Centers - how is it going?</li>
<li> <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Jun/0075.html">Max's JS file import</a></li>
<li> <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Jun/0174.html">revamping flags!</a></li>
<li> Anything blocking you from creating great content?</li>
<li> Anything new &amp; notable? (Blogs or other communications planned for next week?)</li></ul>
<h2><span class="mw-headline" id="DISCUSSION_7">DISCUSSION</span></h2>
<h4><span class="mw-headline" id="TOPIC:_WPW_-_how_is_it_going.3F_3">TOPIC: WPW - how is it going?</span></h4>
<h5><span class="mw-headline" id="SUBTOPIC:_Who_will_be_a_coordinator_for_the_next_4_weeks.3F">SUBTOPIC: Who will be a coordinator for the next 4 weeks?</span></h5>
<p>People aren't officially signing up to be a coordinator, so Doug is basically signed up for all properties. We need people signed up to help.
It's not that hard to coordinate. Just mark down when people volunteer, help them out. Recruit people actively, on the properties you're coordinating. It's too much for doug on his own; other people are helping out ad hoc, but aren't following through to make sure the contributor has actually completed the work.
Alex signed up for last three weeks in July.
</p><p>ACTION: julee to e-mail list to try to get others to coordinate. (DONE)
</p><p>We're still targeted for end of July for first round of P0 CSS properties. Don't want things to fall apart for lack of resources. There are enough volunteers that people can actually get this thing done. 
ACTION: Eliot to move Seattle Doc Sprint properties to a new table on the WPW page. (DONE)
</p>
<h5><span class="mw-headline" id="SUBTOPIC:_How_should_we_circle_back_around_to_folks_who_have_previously_showed_interest.3F">SUBTOPIC: How should we circle back around to folks who have previously showed interest?</span></h5>
<p>Julee started a CRM spreadsheet 
</p><p>If anyone needs access, e-mail Julee. We won't send out public link because it has e-mail addresses on it.
</p><p>Other things we could do for contributors?
</p><p><br />
Lea sent a link to a site that has a contributor spotlight <a rel="nofollow" class="external free" href="http://thenounproject.com/">http://thenounproject.com/</a>
</p><p>We talked about doing something like that in the past. We should definitely recognize. As a blog post or on the home page. There are a bunch of people.  Contributer "cred"
</p><p>Having a contributor highlight on the site shows visitors that there is an active community.
Be a little careful--some people are rather shy and don't want public exposure
</p><p><br />
We don't have profiles right now to configure that. Ryan needs to fix the user profiles. He's actively working on it--it's a MW bug.
</p><p><br />
Just to reiterate, when Julee and I emailed the people who had been past contributors, saying, "you were in the top 20/3o people". That pulled several people back in. People really responded well to the fact that we were acknowledging their contribution.
</p><p>That model is very useful. Even like FitBit sends out little emails to congratulate.
</p><p>shepazu to prod the discussion about recognizing contributors on the mailing list and look for an extension to mediawiki to do the sidebar
</p><p>We could have a per-page thing and the overall site notice thing, profiling people who have done a lot of stuff.
People like Garbee and Max have done a great job, really gone above and beyond.
Either in the TYPE of thing they've done, or the AMOUNT of work they've done
There's a number of bots at Wikipedia that detect things like this automatically
</p><p><br />
Because we need to explicitly let people opt in at this time, it would be just adding a little section on the home page manually. That would be easier to get going.
We do want to execute on the leaderboards thing. It's an automatic way to get people's constructive competition going, if you're #3, you want to reach #2
gamification kicks in…
</p><p>We should talk about all of these analytics in the analytics meeting. i'm going to make a note of these.
</p>
<h5><span class="mw-headline" id="SUBTOPIC:_What_MBF_for_CSS_properties.3F">SUBTOPIC: What MBF for CSS properties?</span></h5>
<p>compatibility tables
data types &amp; units done
get the code samples switched from MSDN to code.webplatform.org
</p><p>checklist to make it quick to review
some kind of visual, or UI indication of whether or not any given page is ready or not
</p><p>a template added to the top like <a href="/w/index.php?title=Template:NeedsWork&amp;action=edit&amp;redlink=1" class="new" title="Template:NeedsWork (page does not exist)">Template:NeedsWork</a> is helpful for "not ready yet"; visitors and new contributors are not sure what 'flags' means
</p><p>a high-level gut check as a group before we go forward
</p><p>high-level CSS WG review, even just flagging issues
I think it should be done, maybe even fairly soon
they might suggest ways in which we should be changing the pages overall
at the docsprint there were a few people from the CSSWG. They had some good review comments. Alan Stearns, Arron Eicholz. Some of them required template changes, like animatable is not a simple boolean unfortunately. Some of them were stylistic
</p><p>Arron Eicholz has many more suggestions.
</p><p>ACTION: shepazu to following up with CSS WG review  -- especially Arron Eicholz , who was in the IRC for this meeting -- to get more suggestions on CSS properties pages
</p><p>review from famous devrel people, they have good reach?
</p><p>people like paul irish or Chris... coyier (sp?)
</p><p><br />
ACTION: jkomoros to work with Paul Irish to coordinate getting devrel type folks to review the docs.
</p><p><br />
ACTION: Lea to incorporate Chris Coyers UI feedback (<a rel="nofollow" class="external free" href="http://lists.w3.org/Archives/Public/public-webplatform/2013May/0241.html">http://lists.w3.org/Archives/Public/public-webplatform/2013May/0241.html</a>)
</p><p>a launch plan
make sure we're contextualizing what we consider this launch to be
</p><p>ACTION: jkomoros to help coordinate a launch plan once we decide to go forward with launch.
</p>
<h4><span class="mw-headline" id="TOPIC:_Max.27s_JS_file_import">TOPIC: Max's JS file import</span></h4>
<p><a rel="nofollow" class="external free" href="http://dev.maxpolk.org/msdnjs/index.php?title=Special:AllPages&amp;from=Constants&amp;to=Objects%2Farguments">http://dev.maxpolk.org/msdnjs/index.php?title=Special:AllPages&amp;from=Constants&amp;to=Objects%2Farguments</a>
Max has a link to first full upload: <a rel="nofollow" class="external free" href="http://dev.maxpolk.org/msdnjs/index.php?title=Special%3AAllPages&amp;from=Objects%2Farguments&amp;to=&amp;namespace=0">http://dev.maxpolk.org/msdnjs/index.php?title=Special%3AAllPages&amp;from=Objects%2Farguments&amp;to=&amp;namespace=0</a>
<a rel="nofollow" class="external free" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Jun/0075.html">http://lists.w3.org/Archives/Public/public-webplatform/2013Jun/0075.html</a>
</p><p>Chrismills and scottrowe, as content architects, give an official response?
They may not be available right now.
</p><p>We should have a calendar or something.
</p><p>ACTION: julee to create a high-level calendar for people to mark when they're available or not. (DONE: <a rel="nofollow" class="external free" href="https://www.google.com/calendar/render?tab=oc&amp;pli=1&amp;gsessionid=P71QgXQ4uw2jGWqFWW6lLA">https://www.google.com/calendar/render?tab=oc&amp;pli=1&amp;gsessionid=P71QgXQ4uw2jGWqFWW6lLA</a>)
</p><p>Limited resources on JS, but other things we can do to support this project?
</p><p>Max is a software developer at ATT mobility. When someone says "we could try one way or another", someone needs to TRY and see if it works.
</p><p>Need folks to review and try the proposals Max is putting out in email.
</p><p>Max needs to explicitly state what he needs.
</p><p>We need a template.
</p><p><br />
frozenice, is just too slammed
</p><p>All template ninjas are too busy.
</p><p><br />
</p><p>ACTION: shepazu to mock up types of JS pages with examples, so we can think about templates from there.
</p><p>We do have tools to edit a page programmatically after the fact, and do mass page renaming, so we should just go forward with it.
</p><p>ACTION: Max to configure the project page with the tasks.
ACTION: Julee to rally an IA overview (DONE)
</p><p>ACTION: shepazu and maxpolk to meet up in person to work on JS page organization
</p>
<h4><span class="mw-headline" id="TOPIC:_revamping_flags.21">TOPIC: revamping flags!</span></h4>
<p>Eliot provided last set of flags that we had settled on
We should go ahead and do it; enough people concurred
</p>
<h4><span class="mw-headline" id="TOPIC:_Demian.27s_Tech_Centers_-_how_is_it_going.3F">TOPIC: Demian's Tech Centers - how is it going?</span></h4>
<p>The general overview is that blackberry is paying for some time to use these tech centers in brazil (schools that are paid to do lab time, basically interns). 4 students who have signed on to take on editing/ css properties. Julee and I met with them last week, will meet again on Monday. 
</p><p>we have four people who will spend 20% of their time a week working on WPD, with Blackberry sponsoring.
University students. They have ten sites. This is a pilot.
</p><p>They have a separate table on WPW <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/Meta:web_platform_wednesday#BlackBerry_Tech_Centers">http://docs.webplatform.org/wiki/Meta:web_platform_wednesday#BlackBerry_Tech_Centers</a>
Interested in being part of the community as we go through. You might see e-mails, or IRC. Down the road, we hope more of the tech centers will help out. 
Millo said Microsoft has similar programs, so once this gets going, we can add on some Microsoft sites.
</p><p><br />
They're mostly CS students, so maybe can help with infrastructure.
</p>
<h4><span class="mw-headline" id="TOPIC:_Anything_new_.26_notable.3F">TOPIC: Anything new &amp; notable?</span></h4>
<p>(Blogs or other communications planned for next week?)
ACTION: Eliot to write up blog post about Seattle Doc Sprint. (DONE)
</p><p><br />
</p><p><br />
</p>
<h2><span class="mw-headline" id="ACTION_ITEMS_8">ACTION ITEMS</span></h2>
<ul><li> julee to e-mail list to try to get others to coordinate. (DONE)</li>
<li> Eliot to move Seattle Doc Sprint properties to a new table on the WPW page. (DONE)</li>
<li> shepazu to following up with CSS WG review  -- especially Arron Eicholz , who was in the IRC for this meeting -- to get more suggestions on CSS properties pages</li>
<li> jkomoros to work with Paul Irish to coordinate getting devrel type folks to review the docs.</li>
<li> Lea to incorporate Chris Coyers UI feedback (<a rel="nofollow" class="external free" href="http://lists.w3.org/Archives/Public/public-webplatform/2013May/0241.html">http://lists.w3.org/Archives/Public/public-webplatform/2013May/0241.html</a>)</li>
<li> jkomoros to help coordinate a launch plan once we decide to go forward with launch.</li>
<li> julee to create a high-level calendar for people to mark when they're available or not. (DONE <a rel="nofollow" class="external free" href="https://www.google.com/calendar/render?tab=oc&amp;pli=1&amp;gsessionid=P71QgXQ4uw2jGWqFWW6lLA">https://www.google.com/calendar/render?tab=oc&amp;pli=1&amp;gsessionid=P71QgXQ4uw2jGWqFWW6lLA</a>)</li>
<li> shepazu to mock up types of JS pages with examples, so we can think about templates from there.</li>
<li> Max to configure the JS project page with the tasks.</li>
<li> Julee to rally an IA overview of Max's JS emails (in progress. PhishtucK is doing great.)</li>
<li> shepazu and maxpolk to meet up in person to work on JS page organization</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="Agenda_2013-06-21:_Meeting_canceled_due_to_lack_of_quorum">Agenda 2013-06-21: Meeting canceled due to lack of quorum</span></h2>
<h2><span class="mw-headline" id="Agenda_2013-06-14:_Meeting_canceled_due_to_lack_of_quorum">Agenda 2013-06-14: Meeting canceled due to lack of quorum</span></h2>
<h2><span class="mw-headline" id="Agenda_2013-06-07">Agenda 2013-06-07</span></h2>
<ul><li> Roll call</li>
<li> Demian Borba of Blackberry and his university program.</li>
<li> Review of open action items</li>
<li> <a href="/wiki/Meta:web_platform_wednesday" title="Meta:web platform wednesday">WPW</a> - how is it going?
<ul><li> How's video going</li>
<li> should we ask Hiroki Yamada to repost announcements to public-webplatform-jp@w3.org?</li></ul></li>
<li> Ryan Lane upgraded site.</li>
<li> <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Jun/0024.html">Naming conventions thread</a></li>
<li> Anything blocking you from creating great content?</li>
<li> Anything new &amp; notable? (Blogs or other communications planned for next week?)</li></ul>
<h3><span class="mw-headline" id="DISCUSSION_8">DISCUSSION</span></h3>
<h4><span class="mw-headline" id="TOPIC:_Demian_Borba_of_Blackberry_and_his_university_program">TOPIC: Demian Borba of Blackberry and his university program</span></h4>
<p>Demian Borba has a webkit implementation in our phone
</p>
<ul><li> … focusing on HTML5</li>
<li> … want to make developers successful</li>
<li> … started a program called Blackberry Tech Center</li>
<li> … Brazil, Argentina, US</li>
<li> … find professors, pick 10 tech students to sponsor</li>
<li> … could donate 20% of time to Web Platform Docs</li>
<li> … in Brazil, we have 5 tech centers</li>
<li> …. 1 in Argentina, Mexico, US</li></ul>
<p>WPD could do project demand for them; provide a weekly structure and set of directions, that would be great.
</p><p>Students are comfortable in EN and comfortable editing articles?
</p><p>Students could also help with software? Kuma, Gollem &amp; GitHub? Some tech centers that are really focused on UX, another on trolling &amp; APIs, for example: blackberry command lines were moved to a UI.
</p><p>It would be great to have them first work on content so they understand the work flow and requirements, and since they're ready to go
</p><p>Community Dev folks will meet with Demian next week. And he can get them to meet once we have execution plan 
</p><p>Millo is looking forward to Tuesdays meeting, can bring in MS similar programs, let's federate the students!
</p><p>shepazu to send email to most active users DONE
</p><p>shepazu to reach out to Kuma ops (Aly). Yes, but no progress
</p><p>shepazu to post on job sites and sysops lists Carry forward
</p><p>julee to ask direct and actionable question on IRC at 11am n/a (DONE)
</p><p>shepazu to send email to most active users - DONE
</p><p>shepazu to reach out to Kuma ops (Aly) - DONE no reply yet
</p><p>julee to ask direct and actionable question on IRC at 11am - KINDA SORTA
</p>
<h4><span class="mw-headline" id="TOPIC:_WPW_-_how_is_it_going.3F_4">TOPIC: WPW - how is it going?</span></h4>
<p>scott is working on video
</p><p>snafu this week, we didn't realize that Scott had already done Flexbox….
</p><p>… so we pulled together an examples week
</p><p>… gathered together things that hadn't been done
</p><p>… on Monday, we're going to work with Nic deCosta, and set forward the next several weeks
</p><p>we meant to put things together earlier, having a set plan in place will give us consistency, we can write blog posts in advance
</p><p>…also folks can do things in advance and have it done by the designated week.
</p><p>…NicDaCosta is in EU; announcing at 11am on Wednesday PDT, kills it for EU; asked that we announce it late Tuesday night, early Wednesday morning
</p><p>..so folks can do it on Wednesday.
</p>
<h4><span class="mw-headline" id="TOPIC:_Japanese_email_list">TOPIC: Japanese email list</span></h4>
<p>julee: should we ask Hiroki Yamada to repost announcements to public-webplatform-jp@w3.org?
</p>
<h4><span class="mw-headline" id="Topic:_Naming_Conventions">Topic: Naming Conventions</span></h4>
<p>julee_: we should be consistent about where landing pages are located
</p><p>shepazu: let's move forward with our master list of topic locations
</p><p>julee_: should Ben Lobaugh do it?
</p><p>Eliot: I'll do it
</p><p>shepazu: ben was also trying to link to the talk page for pointer events
</p>
<h4><span class="mw-headline" id="Topic:_Anything_blocking_you_from_creating_great_content.3F">Topic: Anything blocking you from creating great content?</span></h4>
<p>shepazu: We got an upgrade on MW; some folks have seen some weird quirks - please continue to report anything strange
</p>
<h4><span class="mw-headline" id="TOPIC:_Doc_Sprints">TOPIC: Doc Sprints</span></h4>
<p>MS is having a Doc Sprint 6/22
</p><p>Brazil Doc Sprint TBD
</p><p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Community/Community_Events">http://docs.webplatform.org/wiki/WPD:Community/Community_Events</a>
</p>
<h3><span class="mw-headline" id="ACTION_ITEMS_9">ACTION ITEMS</span></h3>
<ul><li> CARRIED FORWARD: shepazu to post on job sites and sysops lists</li>
<li> shepazu &amp; julee to do a promo check list, including concrete details on how stewards can propagate (Eliot is working on this)</li>
<li> Millo to cc shepazu on his email to new IEEE contact</li>
<li> shepazu to ask Hiroki to propagate announcements to the JP list</li>
<li> We will blog and tweet WPW late Tuesday night</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="Agenda_2013-05-31">Agenda 2013-05-31</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> <a href="/wiki/Meta:web_platform_wednesday" title="Meta:web platform wednesday">WPW</a> - how is it going?
<ul><li> Coordinators finding contributors?</li>
<li> Topic clusters done with instrux?</li>
<li> How's video going</li></ul></li>
<li> <a href="/wiki/Special:RecentChanges%26limit%3D300%26days%3D1" class="new" title="Special:RecentChanges&amp;limit=300&amp;days=1 (page does not exist)">Spam</a> fixing?</li>
<li> Anything blocking you from creating great content?</li>
<li> Anything new &amp; notable? (Blogs or other communications planned for next week?)</li></ul>
<h3><span class="mw-headline" id="Discussion_9">Discussion</span></h3>
<h4><span class="mw-headline" id="TOPIC:_DevOps">TOPIC: DevOps</span></h4>
<p>Recruiting is going slowly.
</p><p><br />
</p>
<h4><span class="mw-headline" id="TOPIC_WPW">TOPIC WPW</span></h4>
<p>coordinators should socialize the list each week
</p><p>coordinators need more time to reach out to contributors: do topics earlier
</p><p><br />
</p><p>problem: many people are not joining the e-mail list
</p><p>A lot of people already have email overload.
</p><p>project.webplatform.org was partially to cure that; there people can jump on and join an issue's discussion
jswisher said mail list is not part of site: not one experience; psychological barrier to "subscribing to an e-mail list"
</p><p><a rel="nofollow" class="external free" href="http://www.discourse.org/">http://www.discourse.org/</a> contextual chatting
</p><p>But, we already have a few systems up that don't talk well with one another.
</p><p>Garbee is working on an actual working Proof of Concept for a new 'wiki' engine. He will share his PoC next week.
</p><p><br />
Denis spent some time trying to get Kuma to work. Persona was a block.
</p><p><br />
We couldn't figure out how to make a page in Kuma
</p><p>If Kuma is worth it, could someone help us from the Kuma community?
</p><p>Imagine this as our editor: <a rel="nofollow" class="external free" href="http://jejacks0n.github.io/mercury/">http://jejacks0n.github.io/mercury/</a>
</p><p>[09:25:07] &lt;julee&gt; jswisher: devs are helpful, but doesn't know about how things would work from the outside.
</p>
<pre>scottrowe worked with mindtouch before <a rel="nofollow" class="external free" href="http://www.mindtouch.com/">http://www.mindtouch.com/</a>
</pre>
<p><br />
we're not going to move forward on a system without having a dedicated devops person.
</p><p>ACTION: shepazu: get ahold of Kuma to get an evaluation copy going
</p><p><br />
Garbee is trying to rope people in from other communities he frequents. A few have shown interest in helping and at least one has already started (brbcoding).
</p><p>go on IRC and ask: who's here right who can help
</p><p>what are the 100 folks on webplatform doing? Lurking.
</p><p>We also had major noise/spam issues right after launch. So, in us trying to control those issues we may have scared people off.
</p><p><br />
IRC people don't like to be told what specifically to discuss. If you are too strict on things, you end up like #html and people don't like you too much.
</p>
<h4><span class="mw-headline" id="TOPC:_Topic_clusters_done_with_instrux.3F">TOPC: Topic clusters done with instrux?</span></h4>
<p>scottrowe has the Action item to of a proposal to create a new set of topic clusters that are pertinent to the page type
</p><p>we need clusters that are relevant to the page type: CSS properties, API, HTML
</p><p>How do we get a specific topic cluster type form field into each page type?
</p><p>scottrowe: we think we can do this, but in the short term, we'll have to have folks put manual links
</p><p><br />
</p>
<h4><span class="mw-headline" id="TOPIC:_WPW_Video">TOPIC: WPW Video</span></h4>
<p>scottrowe has instrux in the video script
</p>
<pre>julee: get a checklist out of script for folks to follow?
</pre>
<p>ACTION: scottrowe to derive a checklist from the video script for editing CSS properties
</p><p><br />
ACTION: scottrowe to send out script to a couple of folks to get feedback before taping.
</p><p>ACTION: scottrowe will tape next week.
</p>
<h4><span class="mw-headline" id="TOPIC:_spam">TOPIC: spam</span></h4>
<p>600+ spam pages
should Admins approve new user creation?
</p><p>ACTION: Garbee and shepazu to get a captcha system that works.
</p><p><br />
[09:58:45] &lt;Garbee&gt; I'd set it up with Questy (with custom questions/answers) to start.
</p><p><a class="external free" href="http://www.mediawiki.org/wiki/Extension:QuestyCaptcha">http://www.mediawiki.org/wiki/Extension:QuestyCaptcha</a> --Something like the first example code.
</p><p><br />
We also need to improve abusefilters.
</p><p>Garbee is working with MicroFormats on sharing stuff once they get their system online.
</p><p>Jswisher said MDN watches the revisions feed and has a dedicated delete; switching to persona has helped - although it might be a temporary effect; Persona for auth is actually a pretty good helper. It, like oAuth, is harder to fake outright.
</p>
<h3><span class="mw-headline" id="Action_Items_10">Action Items</span></h3>
<ul><li> shepazu to send email to most active users</li>
<li> shepazu to reach out to Kuma ops (Aly).</li>
<li> shepazu to post on job sites and sysops lists</li>
<li> julee to ask direct and actionable question on IRC at 11am</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="Agenda_2013-05-24">Agenda 2013-05-24</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> <a rel="nofollow" class="external text" href="http://docs.webplatform.org/test/css/properties/border-radius">ToC</a></li>
<li> <a href="/wiki/Meta:web_platform_wednesday" title="Meta:web platform wednesday">WPW</a> - how is it going?
<ul><li> New and improved: only one table to fill out! (Master page is what we're pulling from. But <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/Meta:web_platform_wednesday">http://docs.webplatform.org/wiki/Meta:web_platform_wednesday</a> will become the final master list.)</li>
<li> We have a standing IRC meeting at 11am PDT, Wednesdays, on #webplatform -- but nothing seems to be happening there.
<ul><li> We should be active on IRC at that time, at least promoting the current week's blog post, and let folks know we're available to answer any questions at that time.</li></ul></li>
<li> What is workflow for WPWs?
<ol><li> Shepazu to pick topic.</li>
<li> Blog written on Tuesday, promo'd Wednesday morning.</li>
<li> Coordinators get volunteers and sign folks up on the WPW page, adding "In Progress"</li>
<li> Coordinators help contributors do properties.</li>
<li> Coordinators should update tables by Tuesday, with "Done" or "Not done".</li></ol></li>
<li> Anyone going to <a rel="nofollow" class="external text" href="http://cssconf.com/">CSSConf</a>? Any opportunity to promote WPW?</li></ul></li>
<li> <a href="/wiki/WPD:Project_Status" title="WPD:Project Status">Getting to Beta</a>
<ul><li> The bug genie is returning connection errors. Seems to be associated with writing certain files.</li>
<li> How to mark bugs that are not in beta - postponed?</li></ul></li>
<li> <a rel="nofollow" class="external text" href="https://docs.google.com/spreadsheet/ccc?key=0Ao_fDuA-PPFydE9vbkR4UWpPRHNjaGFxcjA5WXd5SVE#gid=0">changing www page to focus on community</a></li>
<li> Embedding external pages in WPD? (If Lea's not here, move to next week.)</li>
<li> Anything blocking you from creating great content?</li>
<li> Anything new &amp; notable? (Blogs or other communications planned for next week?)</li></ul>
<h3><span class="mw-headline" id="DISCUSSION_10">DISCUSSION</span></h3>
<h4><span class="mw-headline" id="TOPIC:_Scott_to_do_a_video_on_how_to_do_a_CSS_property">TOPIC: Scott to do a video on how to do a CSS property</span></h4>
<p>It would be cool if people could share tips about doing CSS properties for the video
If we tell people to not fill in compat table information, make sure to emphasize the compat NOTES section
Let's talk about more examples for video, too.
</p><p><br />
We can easily do other ones in the future about how to edit wiki, contribute, etc
</p>
<h4><span class="mw-headline" id="TOPIC:_ToC">TOPIC: ToC</span></h4>
<p>mockup: <a rel="nofollow" class="external free" href="http://docs.webplatform.org/test/css/properties/border-radius">http://docs.webplatform.org/test/css/properties/border-radius</a>
</p><p>Lea pulled ToC out to the side.
</p><p>Suggestions on how to make it better, but acceptable to deploy for now? Yes.
</p><p><br />
</p>
<h4><span class="mw-headline" id="TOPIC:_Web_Platform_Wednesdays">TOPIC: Web Platform Wednesdays</span></h4>
<pre><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/Meta:web_platform_wednesday">http://docs.webplatform.org/wiki/Meta:web_platform_wednesday</a>
</pre>
<p><br />
now coordinators have only one table to update.
</p><p>Shepazu is still tweeking it.
</p><p>Stuff that doesn't get done, gets pushed to next week, or goes back to the hopper to come back in later weeks.
</p><p>coordinator's job is NOT to do all these tasks. The corodinator is supposed to go out and actively recruit people to work on their items. If they can't get anybody, then sure work on them themselves.
</p><p>Master list of what hasn't been done:
<a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/Meta:web_platform_wednesday/master_list">http://docs.webplatform.org/wiki/Meta:web_platform_wednesday/master_list</a>  or <a rel="nofollow" class="external free" href="https://docs.google.com/spreadsheet/ccc?key=0AkRs-89PKiZpdE0xdm9Sb1ZvRW1ZRzMtWEdyU0Z4OEE#gid=14">https://docs.google.com/spreadsheet/ccc?key=0AkRs-89PKiZpdE0xdm9Sb1ZvRW1ZRzMtWEdyU0Z4OEE#gid=14</a> 
</p><p>Master list of what has been done:
<a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/Meta:web_platform_wednesday">http://docs.webplatform.org/wiki/Meta:web_platform_wednesday</a> 
</p><p><br />
ONLY COORDINATORS should fill out that table
</p><p><br />
Workflow is:
</p>
<ol><li> Shepazu to pick topic.</li>
<li> Blog written on Tuesday, promo'd Wednesday morning.</li>
<li> Coordinators get volunteers and sign folks up on the WPW page, adding "In Progress"</li>
<li> Coordinators help contributors do properties.</li>
<li> Coordinators should update tables by Tuesday, with "Done" or "Not done".</li></ol>
<p>We should get topic clusters determined more in advance? like two or three week out
</p><p>Leaverou will speak about WPW at <a rel="nofollow" class="external free" href="http://cssconf.com/">http://cssconf.com/</a>
</p>
<h4><span class="mw-headline" id="TOPIC:_landing_page.2Fhome_page_for_site">TOPIC: landing page/home page for site</span></h4>
<p><a rel="nofollow" class="external free" href="https://docs.google.com/spreadsheet/ccc?key=0Ao_fDuA-PPFydE9vbkR4UWpPRHNjaGFxcjA5WXd5SVE#gid=0">https://docs.google.com/spreadsheet/ccc?key=0Ao_fDuA-PPFydE9vbkR4UWpPRHNjaGFxcjA5WXd5SVE#gid=0</a>
</p><p>General idea: current goal is to get people active, so show community activity!
</p><p>Changes should be done incrementally.
</p><p><br />
</p>
<h4><span class="mw-headline" id="TOPIC:_Beta">TOPIC: Beta</span></h4>
<p>Connection errors on project.webplatform.org are preventing triaging of bugs.
</p><p>In order to easily and quickly view bugs for current milestone within each project's open bugs page, bugs that are not part of the beta should be set to postponed.
</p><p><br />
</p>
<h4><span class="mw-headline" id="TOPIC:_Embedding_external_pages_in_WPD">TOPIC: Embedding external pages in WPD</span></h4>
<p>it would be cool if we could add screencaps from other pages
leaverou  got this from the cubic-bezier page, somebody added screencaps from my tool cubic-bezier.com. She asked him if he thought it was a good idea to embed the tool (assuming I added media queries to make it look good on small viewports). She's wondering if it's possible and allowed.
</p><p><br />
</p>
<h3><span class="mw-headline" id="ACTION_ITEMS_11">ACTION ITEMS</span></h3>
<ul><li> julee to start thread on where new guides exist, where to link them to and what to call them (our Ed, Getting Started, WPW, and Coordinator's guides have confusing names and do not properly reference each other.)  (DONE)</li>
<li> Scott to do a video on how to edit a CSS properties page.</li>
<li> Leaverou to email about embedding a screencaps tool. (CARRIED FORWARD)</li>
<li> shepazu to write up guide on what coordinators do on WPW</li>
<li> leaverou to work on home page design, with the goal of highlighting community activity (CARRIED FORWARD)</li>
<li> shepazu to figure out what connection bug is in project.webplatform.org</li>
<li> Julee to write up an email about "postponing" non-beta bugs.  (DONE)</li>
<li> shepazu to figure out what connection bug is in project.webplatform.org</li>
<li> (CARRIED FORWARD) leaverou to send out e-mail asking people to vote on which skin bugs are more important (DONE)</li>
<li> (CARRIED FORWARD) shepazu to e-mail ML about latest plans for talk.webplatform.org (CARRIED FORWARD)</li>
<li> (CARRIED FORWARD) shepazu &amp; leaverou to mock up what the improved flags will look like. (CARRIED FORWARD)</li>
<li> (CARRIED FORWARD) shepazu to ensure forums banner explicitly states it's for accessibility question only. (CARRIED FORWARD)</li>
<li> (CARRIED FORWARD) shepazu writes down "How to review a page" and the workflow, so coordinators and contributors know what to do and workflow for whole WPW ideally (CARRIED FORWARD)</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="2013-05-17:_Meeting_canceled_due_to_lack_of_quorum">2013-05-17: Meeting canceled due to lack of quorum</span></h2>
<h2><span class="mw-headline" id="Agenda_2013-05-10">Agenda 2013-05-10</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> <a href="/wiki/Meta:web_platform_wednesday" title="Meta:web platform wednesday">WPW</a> - how is it going?
<ul><li> Coordinators:
<ul><li> Doug: </li>
<li> Chris: did all of his, himself -- next time will get others to help</li>
<li> Julee: did some, got help with border-color and examples</li>
<li> Scott: </li>
<li> Janet: </li></ul></li>
<li> Process:
<ul><li> Coordinators please:
<ul><li> update <a href="/wiki/Meta:web_platform_wednesday" title="Meta:web platform wednesday">WPDW</a> main page with assigned items having check marks</li>
<li> update <a href="/wiki/Meta:web_platform_wednesday/2013-05-08" title="Meta:web platform wednesday/2013-05-08">this week's page</a> with status</li>
<li> update <a href="/wiki/Meta:web_platform_wednesday/master_list" title="Meta:web platform wednesday/master list">master list</a> when things are done</li></ul></li>
<li> Doug is working on a <a href="/wiki/Meta:web_platform_wednesday/coordinator_guide" title="Meta:web platform wednesday/coordinator guide">coordinator's guide</a></li>
<li> Do all pages need a different reviewer? At least a "peer" review?</li></ul></li></ul></li>
<li> <a href="/wiki/WPD:Project_Status" title="WPD:Project Status">Getting to Beta</a>
<ul><li> Bug count: 141</li>
<li> How to mark bugs that are not in beta - postponed?</li></ul></li>
<li> Onboarding
<ul><li> Need a stock response to people like Konstantinos who reach out to the list and want to join. And maybe a rotating member of the community team to send them?</li></ul></li>
<li> Any updates?
<ul><li> We have ToCs!</li></ul></li>
<li> <a rel="nofollow" class="external text" href="https://docs.google.com/spreadsheet/ccc?key=0Ao_fDuA-PPFydE9vbkR4UWpPRHNjaGFxcjA5WXd5SVE#gid=0">changing www page to focus on community</a></li>
<li> Anything blocking you from creating great content?</li>
<li> Anything new &amp; notable? (Blogs or other communications planned for this week?)</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="DISCUSSION_11">DISCUSSION</span></h2>
<h3><span class="mw-headline" id="TOPIC:_W3C_accessibility_folks_to_use_our_forums">TOPIC: W3C accessibility folks to use our forums</span></h3>
<p>We need to ensure forums banner explicitly states it's for accessibility question only.
</p><p>There is a cost to everything we maintain. We'd de-emphasize it from the site (well, we already have). The accessibility people have a dedicated, funded person to fund the boards.
</p>
<h3><span class="mw-headline" id="TOPIC:_WPD_Wednesdays">TOPIC: WPD Wednesdays</span></h3>
<p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/Meta:web_platform_wednesday">http://docs.webplatform.org/wiki/Meta:web_platform_wednesday</a>
</p>
<h4><span class="mw-headline" id="WPDW_Status">WPDW Status</span></h4>
<p>We're in good shape, 25 knocked out this week, someone committed for everything but outlines
</p><p>jkomoros can't come next week because of I/O, but have it blocked on my calendar going forward
</p><p>Let's remember to send out inspirational articles when we blog about topics we're focusing on.
</p><p>Weekly cycle is over on Tuesday.
</p><p><br />
</p>
<h4><span class="mw-headline" id="Do_all_pages_need_a_different_reviewer.3F_At_least_a_.22peer.22_review.3F">Do all pages need a different reviewer? At least a "peer" review?</span></h4>
<p>Important that the person who reviews the page is not the person who worked on it.
</p><p>Review shouldn't come across as too much of a blocker. Don't want it to be counter productive
</p><p>Informal coordinator review, peer review, with official tech review later in 1.0 perfect cycle. We should not declare failure if we don't get review. Set review flag, and reviewers clear it. When flags are removed, that shows the pages are the quality that should be standard
</p><p>Peer review to make sure the checklist is taken care of.
Coordinator can do the checklist review
</p><p>If the coordinator can't do it, maybe just pair writers together
</p><p>Technical review for correctness and example is correct
</p><p>Two different levels of review might make the procedure too long winded. Expert review should come later, if needed.
</p><p><br />
The whole point of this exercise is to... get the work done, but mainly to grow contributor base, make it clear how to contribute.
</p><p>some people have already spoken up and started contributing because this makes it easier. Don't take the work away from other people if you can help develop them. It will take some effort to get people into the habit of contributing and building up the contributor base
</p>
<h4><span class="mw-headline" id="Coordinators_responsibilities">Coordinators responsibilities</span></h4>
<p>Doug is working on a coordinator's guide
</p><p>WPDW will be on #webplatform NOT #webplatform-site
</p><p><br />
All coordinators should:
</p>
<ul><li> update WPDW main page with assigned items having check marks</li>
<li> update this week's page with status</li>
<li> update master list when things are done</li></ul>
<p>Coordinators should still do one page. That helps them understand what the pain points are.
</p><p>Coordinators have 1 or 2 volunteers for each WPDW
</p><p>When we have a short-hand property that encompasses all of the other properties for individual settings
</p><p>That's why we chose more properties this week, to keep shorthand/longhand sets together. One person can write the individual longhand properties (which may be in more than one shorthand property), and then do the short hand version.
</p><p>A lot of pages in mine that said, "just see short hand page". That's annoying to click through. Because we don't have transclusion, we should copy paste.
</p><p><br />
</p>
<h3><span class="mw-headline" id="TOPIC:_Getting_to_beta">TOPIC: Getting to beta</span></h3>
<p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Community/Meetings/General#Project_Status">http://docs.webplatform.org/wiki/WPD:Community/Meetings/General#Project_Status</a>
</p><p>The project leads to review the criteria and update the bugs
Extended deadline until mid week next week
</p>
<h4><span class="mw-headline" id="Project_Status">Project Status</span></h4>
<p><a href="/wiki/WPD:Project_Status" title="WPD:Project Status">Project Status Page for Getting to Beta</a>
</p><p>Bug count: 141
</p>
<table class="wikitable" style="text-align: center; width:50%">
<tr>
<th>Project
</th>
<th>Lead
</th>
<th>Open Issues
</th>
<th>Beta defined
</th>
<th>beta bugs assigned
</th></tr>
<tr>
<td>Analytics
</td>
<td>patrickdsouza
</td>
<td>10
</td>
<td>Yes
</td>
<td>Yes
</td></tr>
<tr>
<td>Blog
</td>
<td>Eliot-MSFT
</td>
<td>4
</td>
<td>Yes
</td>
<td>Yes
</td></tr>
<tr style="font-style: italic; color: red;">
<td>commentsextension
</td>
<td>shepazu
</td>
<td>8
</td>
<td>???
</td>
<td>???
</td></tr>
<tr>
<td>community
</td>
<td>jswisher
</td>
<td>1
</td>
<td>Yes
</td>
<td>Yes
</td></tr>
<tr>
<td>compatibilitytables
</td>
<td>shepazu
</td>
<td>1
</td>
<td>Yes
</td>
<td>Yes
</td></tr>
<tr style="font-style: italic; color: red;">
<td>content
</td>
<td>Julee
</td>
<td>40
</td>
<td>Yes
</td>
<td>in progress
</td></tr>
<tr>
<td>dabblet
</td>
<td>Lea
</td>
<td>2
</td>
<td>Yes
</td>
<td>Yes
</td></tr>
<tr style="font-style: italic; color: red;">
<td>InfoArch
</td>
<td>Scottrowe
</td>
<td>9
</td>
<td>Yes
</td>
<td>Yes
</td></tr>
<tr style="font-style: italic; color: red;">
<td>infrastructure
</td>
<td>shepazu
</td>
<td>14
</td>
<td>Yes
</td>
<td>???
</td></tr>
<tr style="font-style: italic; color: red;">
<td>prmg
</td>
<td>Garbee
</td>
<td>17
</td>
<td>Shooting for 5/15
</td>
<td>Shooting for 5/15
</td></tr>
<tr style="font-style: italic; color: red;">
<td>Q&amp;A
</td>
<td>shepazu
</td>
<td>2
</td>
<td>???
</td>
<td>???
</td></tr>
<tr>
<td>skin
</td>
<td>Lea
</td>
<td>17
</td>
<td>Yes
</td>
<td>Yes
</td></tr>
<tr style="font-style: italic; color: red;">
<td>templates
</td>
<td>jkoromo
</td>
<td>7
</td>
<td>dependency on content &amp; ia beta definition
</td>
<td>No
</td></tr></table>
<h3><span class="mw-headline" id="TOPIC:_Onboarding">TOPIC: Onboarding</span></h3>
<p>Need a stock response to people like Konstantinos who reach out to the list and want to join. And maybe a rotating member of the community team to send them?
</p><p>Eliot: We're getting a regular stream of new people, asking how they can help. We need a stock mail to send out, and someone on point to respond
</p><p>people should feel comfortable to customize it.
</p><p>Tell them that wiki wednesday is a great way to get started
</p>
<h3><span class="mw-headline" id="ACTION_ITEMS_12">ACTION ITEMS</span></h3>
<ul><li> (CARRIED FORWARD) shepazu to revamp CSS WG e-mail to be call for contributors (DONE) </li>
<li> (CARRIED FORWARD) leaverou to send out e-mail asking people to vote on which skin bugs are more important</li>
<li> (CARRIED FORWARD) shepazu to e-mail ML about latest plans for talk.webplatform.org (CARRIED FORWARD)</li>
<li> (CARRIED FORWARD) shepazu &amp; leaverou to mock up what the improved flags will look like. (CARRIED FORWARD)</li>
<li> (CARRIED FORWARD) shepazu to ensure forums banner explicitly states it's for accessibility question only. (CARRIED FORWARD)</li>
<li> shepazu to consider putting table at the top of the page (DONE)</li>
<li> shepazu send out an email asking for someone to work on outline (DONE)</li>
<li> Julee to update editor's guide with links to WPDW (DONE)</li>
<li> shepazu to start thread on where new guides exists, where to link them to and what to call them (ACTION transferred to Julee)  (DONE)</li>
<li> (CARRIED FORWARD) shepazu writes down "How to review a page" and the workflow, so coordinators and contributors know what to do and workflow for whole WPDW ideally (CARRIED FORWARD)</li>
<li> Scott to write up quick guide on dealing with shorthand properties (ACTION evolved to: Scott to do a video on how to edit a CSS properties page)</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="Agenda_2013-05-03">Agenda 2013-05-03</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> <a href="/wiki/WPD:Project_Status" title="WPD:Project Status">Getting to Beta</a>
<ul><li> We assigned project owners. Those owners should review the beta criteria and update it with what their "group" thinks should be in the beta. </li>
<li> Beta criteria needs to be clarified at the higher level as well. For example:
<ul><li> <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Apr/0370.html">Scott's take</a></li>
<li> We need more folks vetting the content that's there. The community TF will do a recruiting plan.</li>
<li> We need folks to work on content, especially CSS properties pages. We may ask folks to own certain portions, to be divvied up amongst their friends and family, or otherwise focus on that.</li>
<li> For each content area, we should have exemplar content</li>
<li> Each page should be clearly designated as either ready to consume or needing additional contributions.</li></ul></li>
<li> What you can do:
<ul><li> If you're a project leader:
<ul><li> discuss beta criteria with stakeholders and update the Project Status page.</li>
<li> make sure you have tasks and bugs relating to beta in project.webplatform.org, and that they're assigned to someone.</li>
<li> if you find blockers, file a bug, and broadcast it to the public list</li></ul></li>
<li> If you're an individual contributor:
<ul><li> work on some CSS properties</li>
<li> if you find blockers, file a bug, and broadcast it to the public list</li></ul></li></ul></li></ul></li>
<li> CSS Properties pages</li></ul>
<h2><span class="mw-headline" id="DISCUSSION_12">DISCUSSION</span></h2>
<h3><span class="mw-headline" id="TOPIC:_Beta_2">TOPIC: Beta</span></h3>
<p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Community/Meetings/General">http://docs.webplatform.org/wiki/WPD:Community/Meetings/General</a>
<a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Project_Status">http://docs.webplatform.org/wiki/WPD:Project_Status</a>
<a rel="nofollow" class="external free" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Apr/0370.html">http://lists.w3.org/Archives/Public/public-webplatform/2013Apr/0370.html</a>
</p><p>About Beta: we aren't out of the woods until we get to Beta, at that point, we can be comfortable saying "use this content". That's the critical mass point. Watching all the sub-task forces doing their work, it's great, but imagine that there's a day when stewards or others leave and it starts a mass exodus. Get to critical mass: instead of doing so across the site. Set up a beta based on a content category. The beta can apply to one part of the site. There is a risk that if the project does not achieve a measure of usability, stakeholders may lose interest. The CSS properties project was that set that folks could use as a resource. This calls for focusing on content, to the exclusion of other things.
</p><p>This should be a fundamental shift in how we do this. Not beta criteria for all of WPD, but define beta criteria for individual content areas, and define beta status on each bucket. Define "beta" as pertaining to discrete content areas. First "beta": CSS Properties.
</p><p>We need a milestone achievement - CSS Properties. If work doesn't lead to that, defer it. This week, we realized we're spreading our energies too thin. So we should focus our energies on CSS properties project. But, volunteer help is not fungible. For example, Max Polk is willing to work on the MSDN stuff but not interested in other bits. The only thing I would say that needs to be done is:
</p><p>1) have the compatibility tables from MSDN and caniuse working (because that's a big part of content creation and user experience). If people come to the site and don't see consistent compat tables, it doesn't look good. So our work there is better spent finishing up compat extension.
</p><p>2) Also, we need to have an exemplar for each page, which is the criteria we had for beta--that's the other thing we we should have for beta.
</p><p>We all agree on CSS Properties. Other content areas will be deferred.
</p><p>What about other beta tasks?
</p><p>Do we want to go back to the project status page and look at those and say if any of those are direct for beta? If we focus on this stuff and don't try to recruit additional contributors, and we say CSS properties are beta, will we have a site that people can consume and contribute to?
</p><p>Eliot: There are two things there. There's the content effort and the infrastructure effort. (The latter includes compat tables, community, etc.) community growth can still go on, it's separated from what the community is working on. Even MDN is mostly people consuming. Really only about 15 contributors.
</p><p>Want to reframe a bit: "What is beta"&#160;? what are we trying to accomplish? who is the audience?
</p><p>1)	ourselves. To push ourselves and feel momentum
2)	an opportunity to talk to, after the alpha announcement, to engage public and say hey look, another chance to introduce ourselves
3)	is the stewards
</p><p>If we talk about this awesome resource, and we don't have it yet, web developers need to see progress, momentum. if they see value, they'll respond, if devs promote, we're successful. We aren't changing our goals. We need to change focus and messaging for this content only. This was the general plan from the beginning of the CSS properties project?
</p><p>If we do micro-betas, it may dilute the impact of a general beta. It will be virtually impossible for us to get _all_ of the content to beta.
</p><p>But if we have a set of clear, well-defined criteria for the different sections, that shows evidence of progress. So it's the only path to success.
</p><p>Then we need to be clear that we're focused on the _content_, not the _site_. We'll continually revise and refine our processes around recruitment and participation. We've already got a lot more than what we started with. We've made some strides in that area. Some efforts in regard to recruiting may not be timed appropriately to achieve a short-term objective.
</p><p>When Eliot sent the mail out, he was looking at was our loss of focus on the content front. We're putting together a LARGE project with many different facets. At Microsoft, we have a team of writers, and a production team, and a marketing team 
and we don't take marketing people off that when we need to do a content push.
</p><p>We shouldn't do it here. We should identify who's working on what, and what they're doing. The note was really just about loss of focus on Content front. We'll continue to look at bugs and project status page focus on other areas, but as far as content effort goes, we focus on CSS properties. Other aspects are secondary but still important.
</p><p>Folks will review their bugs:
</p><p>Infrastrucutre is Doug. Content is Scott, Chris, and Julee. Community is Janet for beta criteria.
</p><p>Right now, the site notice has a new call to action on JS.
</p>
<h3><span class="mw-headline" id="TOPIC:_CSS_Properties_work">TOPIC: CSS Properties work</span></h3>
<p>The CSS properties sheet is overwhelming folks. <a rel="nofollow" class="external text" href="https://docs.google.com/spreadsheet/ccc?key=0AkRs-89PKiZpdE0xdm9Sb1ZvRW1ZRzMtWEdyU0Z4OEE#gid=17">Julee updated it</a>.
</p><p>We need to ensure that new contributors are properly supported. <a href="/wiki/WPD:CSS_property_guide/supporting_new_contributors#Helping_contributors_with_CSS_properties_page" title="WPD:CSS property guide/supporting new contributors">Plan to help contributors</a>
</p><p>Everyone on this call who's not up for this, e-mail me specifically, otherwise you're on the hook for being an ambassador or greeter.
Weekly content-wrangling events on IRC is being scheduled for the West coast first, as Scott and Julee have already volunteered as consistant facilitators. Please fill out <a rel="nofollow" class="external text" href="http://www.doodle.com/y4bdnrg4ycdk4i25">doodle poll</a>
</p>
<h3><span class="mw-headline" id="TOPIC:_Forums">TOPIC: Forums</span></h3>
<p>w3c accessibility folks want to use our forums. So, let's keep them open, we've already deemphasized them on the site and communications channels. But let's keep them open so accessibility folks can use it.
</p>
<h2><span class="mw-headline" id="ACTION_ITEMS_13">ACTION ITEMS</span></h2>
<ul><li> Shepazu to mock up how project should be represented in the wiki (DONE)</li>
<li> shepazu: update the site notice about the CSS Properties push and how to get started AND use the piwik tracking campaign code.  (DONE)</li>
<li> shepazu to draft up CSS properties project blog post (circulate for comment) AND use the piwik tracking campaign code.  (DONE)</li>
<li> shepazu to revamp CSS WG e-mail to be call for contributors</li>
<li> leads to review the bugs for project areas on project.webplatform.org (jswisher, shepazu, cmills, julee, scottrowe)  (In progress: See: <a href="/wiki/WPD:Community/Meetings/General#Project_Status" title="WPD:Community/Meetings/General">Project Status table</a>)</li>
<li> shepazu to send out e-mail asking people to vote on which skin bugs are more important</li>
<li> shepazu will send an email about change in forums with w3c accessibility folks using it to answer questions</li>
<li> (CARRIED FORWARD) shepazu to e-mail ML about latest plans for talk.webplatform.org </li>
<li> (CARRIED FORWARD) leaverou: to talk with Chris Coyier regarding reviewing css properties template.</li>
<li> (CARRIED FORWARD) leaverou: will follow up with Denis where global nav didn't get implemented.</li>
<li> (CARRIED FORWARD) shepazu to work with lea to mock up what the improved flags will look like.</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="Agenda_2013-04-26">Agenda 2013-04-26</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items.</li>
<li> Appearance of content flags.</li></ul>
<dl><dd> Limited, but pointed feedback (from doc sprinters, others) suggests that these may be a deterrent to editing content. Consider toning them down?</dd></dl>
<ul><li> <a href="/wiki/WPD:Projects/DOM_API_docs" title="WPD:Projects/DOM API docs">DOM API Doc Reorganization Proposal</a>.</li>
<li> Task forces reporting back to this general meeting.</li>
<li> Anything blocking you from creating great content?</li>
<li> Any new or notable content to promote?</li></ul>
<h2><span class="mw-headline" id="DISCUSSION_13">DISCUSSION</span></h2>
<h3><span class="mw-headline" id="TOPIC:_Appearance_of_content_flags">TOPIC: Appearance of content flags</span></h3>
<p>Limited, but pointed feedback (from doc sprinters, others) suggests red flags may be a deterrent to editing content. Consider toning them down?
</p><p>... it's a bit "boy who cried wolf"
</p><p>Should the meaning of flags be explained more explicitly when being set and viewed?
</p><p>Some of them should be stronger than others
</p><p>being able to change the priorities/visibility, and actions that are obvious from them
</p><p>ideally, stub should be more inviting, for example
</p><p>Back at the beginning, the plan was to display them differently to signed in vs signed out people
</p><p>Also, flag banner is broken: <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/html/elements/!DOCTYPE">http://docs.webplatform.org/wiki/html/elements/!DOCTYPE</a>
</p><p>[agreement that this is something to fix]
</p><p><br />
For beta, clear visual representation that this page is considered Beta-ready or not, we won't be able to touch all of the pages for beta
</p><p>That's especially important given that some parts of site will be ready to be called beta before others
</p><p>Could just have a banner that says "flags associated" or "this article is not beta ready", and when you go down to the _bottom_ it shows the flags
</p><p>If you look at the compat table's output, when you mouse over it shows one thing for all mobiles; then when you mouse over it shows details
</p><p>Also, I think a simple tooltip for explanation of flags (on hover) would be sufficient, maybe have popup appear on mobile devices
but something like that that says "there are flags on this page" and when you hover over see the specific ones
</p><p>vs going to a whole separate page
</p><p>... also we haven't done a great job of encouraging a culture of using flags
</p><p>... we need to work those flagged pages back into the work flow
</p><p>Making each flag a call to action could help
</p><p>I think a tooltip explanation on the page whee it happens and a longer explanation linked from the editing page, where you set the flags would work
</p><p>... comments thing was also supposed to help with flagging
</p><p>... we want the comments thing to plug in to the issue tracker. Ideally the flags would go into the issue tracker
</p><p>... ideally on the page you check off, I've done this, it hits the API to issue tracker and says "this action ahs been done"
</p><p><br />
A lot of work, but there could be phases to it. If we can get the current UI to reflect the call to action
</p><p><br />
and then later on hook up to project tracking
</p><p><br />
My original ideas was to have them discrete and off to the sdie
</p><p>... right now they're a banner at the top of most pages
</p><p><br />
Also, if you could be clear about what the workflow should be
</p><p>... in other words, contributor goes to edit the page, see one banner, they click on that, then they see all flags as calls to action...
</p><p><br />
</p>
<h3><span class="mw-headline" id="Topic:_DOM_API_reorganization_proposal">Topic: DOM API reorganization proposal</span></h3>
<p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Projects/DOM_API_docs">http://docs.webplatform.org/wiki/WPD:Projects/DOM_API_docs</a>
</p><p>Adopted with the following discussion:
</p><p>Want to make sure it's predictable and avoids conflicts
Follow basic object hierachy but flatten it out
</p><p>Shepazu provided one example of proper DOM hierarchy:
</p><p><a rel="nofollow" class="external free" href="http://objjob.phrogz.net/">http://objjob.phrogz.net/</a>
</p><p>that lets you drill around all around everywhere within the DOM. I had a vision that all of these things would be interlinked
</p><p>URL schema for DOM API and visual representation of the DOM don't have to be the same thing. There's a lot of depth to the DOM that users don't need exposure to when they're coding. There are two use cases. The one we're solving for primarily is to figure out what a particular method does--they don't care about where it is in the dom tree. But that would address the other use case of exploring
</p><p>We should have a widget that allows you to explore the particular object and its hierarchy as a UI element as opposed to a URL element
</p><p>Are these two problems: 1) URL hierarchy 2) rendering of content to readers?
</p><p><br />
It's about 1200 pages tagged as DOM. And you need to be an admin to do moves
</p><p><br />
We should have a big push where we move the pages.
</p><p>Fr0zenice might know if there's an extension
</p><p><br />
dunno, but the "move only for admins" thing was never really implemented btw
</p><p>We don't want to lose this idea of a visual representation of the DOM. something we could point to as a differentiator. Because there's no good place to see that today
</p><p>What we're documenting here is one ideal reference implementation of all the specs and we can show that to you in this visual way
</p><p>We do want our work on web platform to help people working on standards
</p><p>Not in URL structure, but in a separate experience
</p>
<h3><span class="mw-headline" id="Topic:_Task_force_statuses">Topic:  Task force statuses</span></h3>
<h4><span class="mw-headline" id="Community_Development">Community Development</span></h4>
<p>we firmed up out plans for upcoming doc sprints
</p><p><br />
Any updates to any of the events should be reflected on the <a href="/wiki/WPD:Community/Community_Events" title="WPD:Community/Community Events">events page</a>.
</p><p>shepazu's great idea&#160;: have a non-political description of DRM and DNT, have technical articles about those and make a blog post.
</p><p>... the TECHNICAL aspect, not political, social, or standardization aspect
</p><p>and the ancillary idea was: we have an alpha banner, but we don't have anything about the campaigns we're working on (like CSS properties)
</p><p>... when we have a push, we should highlight them in the banner
</p><p>Redesiging the notice so it's not quite so ugly and what our current call to action
</p><p>So, we have the blog, but do we also need a News or Current Events page linked to from the home page?
</p><p>More controversial topics might get more vandalism, we'll need to be vigilant.
</p><p>And we'll want to make it clear we're trying to just be about TECHNICAL aspects.
</p><p>Have a disclaimer, if you want to discuss social aspects, here are some links for you to go to to do that
</p><p><br />
the blog entry where we say "we realize these are controversial, this is the role we're trying to play"
</p>
<h3><span class="mw-headline" id="TOPIC:_Status_of_CSS_properties_project">TOPIC: Status of CSS properties project</span></h3>
<p>We're stalled on contributors to content. Not too much to review compared to content we need to create
</p><p>We might need to broaden our base to get more contributors
</p>
<h3><span class="mw-headline" id="TOPIC:_compatibility_tables_2">TOPIC: compatibility tables</span></h3>
<p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Compatibility_Info">http://docs.webplatform.org/wiki/WPD:Compatibility_Info</a>
</p><p><br />
There's a disconnect between pages that we have and granularity of caniuse data
</p><p>If we're going to replace our existing compat tables, we'll need to do so comprehensively.
</p><p>MOzilla agreed that we can crawl MDN's compat information, as this is public domain content. They agreed that we can use this data, and are not required to mark it as their _license_, although of course we'll say we got the info from them.
</p><p>Shepazu is working on a script to extract data from them, merge with caniuse
</p><p>If there's a test missing, then we'll provide a simple interface for folks to provide one, or at least some input.
</p><p>if you see something missing, if you want to give the test to help with that
it will take them to a thing to let them contribute a test
</p><p>That's huge overhead, will discourage contributions.
</p><p>But how will we know it's good if they just make an assertion?
</p><p><br />
We can have a way to put in unverified information, but it should be tagged that it needs tests
</p><p><br />
</p>
<h2><span class="mw-headline" id="ACTION_ITEMS_14">ACTION ITEMS</span></h2>
<ul><li> julee to email project leads inviting them to Monday's meeting. (DONE)</li>
<li> pending Alex's amazing, insightful review of the DOM API proposal, Scott to begin implementing (DONE)</li>
<li> Julee to file a bug to get a visual representation of the DOM hierarchy (DONE: <a rel="nofollow" class="external free" href="http://project.webplatform.org/content/issues/46">http://project.webplatform.org/content/issues/46</a>)</li>
<li> Julee to add CSS properties recruting to communications meeting (DONE)</li>
<li> shepazu to propose concrete proposal on compat info to list once it's done (ON-GOING)</li>
<li> shepazu to e-mail ML about latest plans for talk.webplatform.org (CARRY FORWARD)</li>
<li> leaverou: to talk with Chris Coyier regarding reviewing css properties template. (CARRY FORWARD)</li>
<li> leaverou: will follow up with Denis where global nav didn't get implemented. (CARRY FORWARD)</li>
<li> shepazu to work with lea to mock up what the improved flags will look like (CARRY FORWARD)</li></ul>
<h2><span class="mw-headline" id="Agenda_2013-04-19">Agenda 2013-04-19</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> Task forces reporting back to this general meeting:
<ul><li> Community</li>
<li> Analytics</li>
<li> Program Management</li></ul></li>
<li> Anyone want to share any status on any project? Can we get completion dates?</li>
<li> Review proposed URL/structure of <a href="/wiki/WPD:Projects/DOM_API_docs" title="WPD:Projects/DOM API docs">DOM API docs</a>.</li>
<li> Has anyone seen the Evil Session Bug lately?</li>
<li> When you tweet, don't forget to check conversation for follow-up!</li>
<li> Anything blocking you from creating great content?</li>
<li> Any new or notable content to promote?</li></ul>
<h2><span class="mw-headline" id="DISCUSSION_14">DISCUSSION</span></h2>
<h3><span class="mw-headline" id="TOPIC:_CSS_Properties_reviewers">TOPIC: CSS Properties reviewers</span></h3>
<p>Doug and Chris Mills commented. Maybe have design experts join in, but unclear if they were to be SME to review content or the design of the pages.
we did a couple of rounds on the template.
</p><p>We did another round in January, so I don't think we need to review the design further. Does anyone else?
</p><p>Lea's been good about finding optimizations and fixing problems.
</p><p>Joanie Rustalkin who helped design said we could contact her. She'd be an obvious choice.
But let's not revisit design of the template.
</p><p>The idea was to get feedback on the content. But Lea can review design and discuss with other designers, such as Chris Coyier.
</p>
<h3><span class="mw-headline" id="TOPIC:_Compatibility_tables_3">TOPIC: Compatibility tables</span></h3>
<p>May be able to pull in data for mobile, too. <a rel="nofollow" class="external free" href="http://mobilehtml5.org/">http://mobilehtml5.org/</a> <a rel="nofollow" class="external free" href="http://firt.mobi/about.php">http://firt.mobi/about.php</a>
</p><p>Any others?
</p><p><a rel="nofollow" class="external free" href="http://html5test.com/results/desktop.html">http://html5test.com/results/desktop.html</a>
Their methodology did not--ironically-seem test-based. Shepazu to 
contact them anyway.
</p>
<h3><span class="mw-headline" id="TOPIC:_TF_updates:">TOPIC: TF updates:</span></h3>
<h4><span class="mw-headline" id="Community">Community</span></h4>
<p>had a meeting last week
</p><p>university outreach: established a spreadsheet. Will list contact there, but we won't make that public.
</p><p>We will invite people to contribute to that list.
[
We're considering doc sprints. Still working on that.
</p><p>Established a regular meeting time. Tuesdays at 10am Pacific time.
</p><p>If we have an agenda, we'll use the time. Otherwise cancel instance.
</p>
<h4><span class="mw-headline" id="Analytics">Analytics</span></h4>
<p>Topic clusters.
</p><p>Setting up a human readable site map.
We'll track campaign and emails.
</p>
<pre>Before any doc sprint, need to set up a campaign.
</pre>
<p>Our SEO: Setting it up. Next step is to optimize the content. We have this tracked in Bug Genie.
</p>
<h4><span class="mw-headline" id="Program_Management">Program Management</span></h4>
<p>Meetings 11am Pacific time on Mondays.
</p><p>Triaging bugs and gathering information about the state of the beta work.
</p><p>This week we asked people to take ownership of the different project buckets. Owners will define the deliverables and build a time, triaging issues, reporting back to the PM group on progress towards beta.
</p><p>We also talked about BugGenie and how to get reporting done ACROSS projects.
</p><p>Hopefully, we can get away from meetings and get a dashboard look at status.
</p>
<h3><span class="mw-headline" id="TOPIC:_URL_structure_DOM.2C_JS.2C_and_topic_clusters">TOPIC: URL structure DOM, JS, and topic clusters</span></h3>
<p>URL/structure of DOM API docs.
</p><p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Projects/DOM_API_docs">http://docs.webplatform.org/wiki/WPD:Projects/DOM_API_docs</a>
</p><p>follows the same scheme as API docs, but without the API listing pages that describe the common names. Since the common name for all of these is DOM.
</p><p>Doesn't affect how we're going to deal with the JS docs from Microsoft.
</p><p>scottrowe: If folks would review that, it'd be great. I added some more info.
</p><p>You coulld make a case that everything's in the DOM, but that wouldn't help people delineate anything from DOM down.
</p><p>We've done that in our top level buckets , and now we're isolating a subgroup of the DOM and calling that the DOM APIs.
</p><p>.They're the interfaces and objects you use when interfacing with the object model. I can make it clearer in the proposal, but I thought that was an established methodology.
</p><p>this came up earlier, and I hashed it out with some architects. We couldn't come up with a sensible way of doing an alternate view. Scott's proposal is widely accepted.
</p><p>We still need to have some kind of instruction--even visual representation--of the DOm, interfaces, JS, etc.
That might be an article, so then we could explain why we put things places.
</p><p>We haven't talked a lot about interlinking between articles and we should look at that a lot.
</p><p>We should cross-reference related things. MediaWiki doesn't make it as easy as a dedicated documentation CMS, but.
</p><p>We'd talked about topic clusters as doing this.
</p><p>There's an issue filed. Let's use that to discuss this.
</p><p>There may be a passive-aggressive way to make them enter links: topic cluster UI based on links within doc, so if you don't have links, your topic cluster doesn't look right.
</p><p><a rel="nofollow" class="external free" href="http://project.webplatform.org/content/issues/42">http://project.webplatform.org/content/issues/42</a>
</p>
<h3><span class="mw-headline" id="TOPIC:_Session_Bug">TOPIC: Session Bug</span></h3>
<p>MIA Close it!
</p>
<h3><span class="mw-headline" id="TOPIC:_Watch_channel_after_tweeting">TOPIC: Watch channel after tweeting</span></h3>
<p>When you tweet, don't forget to check conversation for follow-up!
</p>
<h3><span class="mw-headline" id="TOPIC:_blogging_about_new_SVG_articles">TOPIC: blogging about new SVG articles</span></h3>
<p>julee: I think Mike Sierra has moved to something else at Adobe. Finished out a bunch of SVG work. HTML5 weekly mentioned the articles.
</p>
<h3><span class="mw-headline" id="TOPIC:_table_styles">TOPIC: table styles</span></h3>
<p>In some pages, there are tables without a class to target. If I style all tables inside the container, it'll have unforseen effects. 
Regarding the font, I am fine changing it. PErsonally, I think bitter looks better.
Is there an automated way to add a class to tables that don't have one?
</p><p>A lot of tables were generated by authors and some use the pipe hack, so there are some issues with tables we generated.
</p>
<h2><span class="mw-headline" id="ACTION_ITEMS_15">ACTION ITEMS</span></h2>
<p>•	leaverou: to talk with Chris Coyier regarding reviewing css properties template. (STATUS: Lea is at a conference right now, and will be mentioning WPD explicitly)
•	leaverou: will follow up with Denis where global nav didn't get implemented. (STATUS: carried forward)
•	shepazu: change the messaging on talk.webplatform.org. (STATUS: not sure that changing messaging is the right thing at this point. Shepazu to send an e-mail to ML)
•	Patrick: to give us optimal day and time to launch a blog post. (DONE)
•	Analytics TF: set up page optimization in the next two weeks. (likely won't happen right now, it's ongoing)
•	Project area leads: join next week's call so we can define what it means to be head of a task force. (STATUS: Meeting didn't happen, due to zakim snafu. Please join us next week.)
</p>
<h2><span class="mw-headline" id="Agenda_2013-04-12">Agenda 2013-04-12</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> April 3 Doc Sprint
<ul><li> How was it?</li></ul></li>
<li> A lot of meetings next week
<ul><li> Community</li>
<li> Analytics</li>
<li> Programming</li></ul></li>
<li> Closing out some items
<ul><li> <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Apr/0121.html">Forum dependencies</a> - completion date?</li>
<li> <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Apr/0090.html">Translation URL schema</a> (<a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/lang/es/Main_Page">http://docs.webplatform.org/wiki/lang/es/Main_Page</a>) - decision final?</li>
<li> <a rel="nofollow" class="external text" href="http://project.webplatform.org/infrastructure/issues/1">Session bug</a> is gone again! Is this issue closed?</li></ul></li>
<li> Anyone want to share any status on any project? Can we get completion dates?
<ul><li> CSS Properties project
<ul><li> Discuss sending out a "call for review"</li></ul></li>
<li> Project.* project</li>
<li> Global nav project</li>
<li> <a rel="nofollow" class="external text" href="http://project.webplatform.org/content/issues/41">Beginners guide</a> to web dev - Status from Chris: created all of the <a href="/w/index.php?title=TEST:beginners&amp;action=edit&amp;redlink=1" class="new" title="TEST:beginners (page does not exist)">landing pages</a> and writing updated text for the landing page</li>
<li> Populating news email list with <a href="/wiki/WPD:Projects/Communications/Universities" title="WPD:Projects/Communications/Universities">university contacts</a>
<ul><li> Fellowships, interships, mentoring programs for students</li>
<li> Please gather university contacts to add to an announce email list</li></ul></li></ul></li>
<li> Anything blocking you from creating great content?</li>
<li> Any new or notable content to promote?</li></ul>
<h3><span class="mw-headline" id="Discussion_15">Discussion</span></h3>
<h4><span class="mw-headline" id="TOPIC:_April_3_Doc_Sprint">TOPIC: April 3 Doc Sprint</span></h4>
<p>It was great. Scott did a blog post about it.
</p>
<h4><span class="mw-headline" id="TOPIC:_A_lot_of_meetings_next_week">TOPIC: A lot of meetings next week</span></h4>
<p>We should confirm that these meetings are productive: resulting in getting work done. If not, we should review.
</p>
<h4><span class="mw-headline" id="TOPIC:_Forums_dependencies">TOPIC: Forums dependencies</span></h4>
<h4><span class="mw-headline" id="TOPIC:_.2A">TOPIC: *</span></h4>
<p>We want to <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Apr/0121.html">close down forums</a>, but we need to get some things done first. See dependencies: 
</p><p><a rel="nofollow" class="external free" href="http://project.webplatform.org/content/issues/40">http://project.webplatform.org/content/issues/40</a>
</p>
<h4><span class="mw-headline" id="TOPIC:_Translation_URL_schema">TOPIC: Translation URL schema</span></h4>
<p>We came close to a decision on the URL schema for other languages:
</p><p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/lang/es/Main_Page">http://docs.webplatform.org/wiki/lang/es/Main_Page</a>
</p><p>But shepazu said we rejected this many times before.
</p><p>What we have now is almost the worst of both worlds. Bad design by W3C LOC experts, MW's auto URL schema isn't good, 
what we're doing now is bad for SEO.
</p><p>Shepazu will follow up with Richard Ishida, W3C's internationalization and localization expert
</p>
<h4><span class="mw-headline" id="TOPIC:_Session_bug_is_gone_again.21">TOPIC: Session bug is gone again!</span></h4>
<p>People haven't seen it, but let's give it a little more time to test.
It was a token bug. There's a token that ID's the session, depending on the memcache. It wasn't able to find the session and the session was lost. Ryan removed single-signon, and changed the memcache server.
</p>
<h4><span class="mw-headline" id="TOPIC:_CSS_Properties_project_2">TOPIC: CSS Properties project</span></h4>
<p>Discuss sending out a "call for review". See [
<a rel="nofollow" class="external free" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Apr/0148.html">http://lists.w3.org/Archives/Public/public-webplatform/2013Apr/0148.html</a> thread].
</p><p>But what's the process? Is Julee the right person to send reviewers to? What does she then do? How do we handle comments, store them, deal with them after we get the review? Seems like we don't have any system. Do we have the list of pages to review?
</p><p>We're talking about SME, we can just ask them to just to edit the page. We won't track what changes they're making. But, what if the change should be made across more pages? So our pages are consistent in org or style?
</p><p>Also, do we have a golden standard? If folks want to talk about specific styles, it's in one location: the golden standard.
Is there a WPD voice? We added the golden standard to the top of the [<a rel="nofollow" class="external free" href="https://docs.google.com/spreadsheet/ccc?key=0AkRs-">https://docs.google.com/spreadsheet/ccc?key=0AkRs-</a>
89PKiZpdE0xdm9Sb1ZvRW1ZRzMtWEdyU0Z4OEE spreadsheet].
</p><p>Julee will work with SME to decide what pages they're going to review. If it's something global, they need to call that out and we need to fix it across the docs. 
</p><p>SMEs are looking for whether he doc is technically accurate.
What we're asking them to determine if the article is "technically accurate?" We're not asking them to set the style of content.
</p><p>So we do need to hand pick some pages to get SME feedback, but once they say a doc is good, that's good enough.
</p><p>We're going to get different voices in a Wiki. But, maybe less so in reference docs. But the priorities are:
</p><p>•	quality content
•	then i18l English
•	Then down the line comes the issue of voice.
So, the ref should be in active voice and some other things, but we shouldn't impose too much at the beginning. Not before we see how things evolve.
</p><p>Let's have as little process as possible. This is our first major writing project, let's put the least process in the beginning and put checkpoints in place later.
</p><p>We should make it clear that SMEs need to let us know if there's something global.
</p><p>And the letter needs to say if they see something that should be fixed across pages, or if they see any problems, contact julee. Want to make it easy for the SMEs to give feedback but doesn't need an official process to make that happen.
</p><p>shepazu: is concerned that we would make a call for review and problems that would cause them not to come back later. this is a push to a larger community than we've had, so we want them to feel satisfied.
</p><p>Julee will send out an email clarifying process. 
</p>
<h4><span class="mw-headline" id="TOPIC:_Project..2A_project">TOPIC: Project.* project</span></h4>
<p>Garbee writing instrux. Having a state view of the beta is a dependency on reporting progress. This can be accomplished with a master project bucket.
</p><p>shepazu: julee &amp; shepazu will follow up
</p>
<h4><span class="mw-headline" id="TOPIC:_Global_nav_project">TOPIC: Global nav project</span></h4>
<p>The <a rel="nofollow" class="external text" href="http://project.webplatform.org/content/issues/14">global nav</a> has not been implemented consistently. Forums closing has a dependencies on this project.
</p><p>Lea's out this week. She's going to point to WPD in her preso!
</p><p><br />
</p>
<h4><span class="mw-headline" id="TOPIC:_Beginners_guide_to_web_dev">TOPIC: Beginners guide to web dev</span></h4>
<p>Chris Mills created all of the landing pages and writing updated text for the landing page.
</p><p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/TEST:beginners">http://docs.webplatform.org/wiki/TEST:beginners</a>
</p><p><a rel="nofollow" class="external free" href="http://project.webplatform.org/content/issues/41">http://project.webplatform.org/content/issues/41</a>
</p><p>Note we have commenting on the issue page! Try to move discussion about implementation to project.* page.
</p>
<h4><span class="mw-headline" id="TOPIC:_Populating_news_email_list_with_university">TOPIC: Populating news email list with university</span></h4>
<p>This is probably a comm &amp; recruiting item. In the meantime, we're asking everyone to please gather university contacts to add to an announce email list.
</p><p>ALSO: Fellowships, interships, mentoring programs for students: GSoC: we got rejected (explicitly not for documentation). But w3c did get approved. Shepazu will follow up.
</p><p>Media Wiki has a mentoring program, can we add our project to their list? Julee will follow up.  (DONE)
</p>
<h4><span class="mw-headline" id="TOPIC:_status_of_table_styles">TOPIC: status of table styles</span></h4>
<p>Lea will incorporate scott's feedback.
</p>
<h4><span class="mw-headline" id="TOPIC:_W3C_WG">TOPIC: W3C WG</span></h4>
<p>W3C WG  is the week after next, may interfere with this meeting. Eliot and Shepazu will talk about presenting there.
</p>
<h4><span class="mw-headline" id="TOPIC:_Compatibility_tables_project">TOPIC: Compatibility tables project</span></h4>
<p>Shepazu has been working on extension with caniuse data; alexsis d. &amp; ppk: quirks mode data is all HTML.
</p><p>PPK will package this data. Shepazu is merging these data sets. We may use MDN data as a fallback for the gaps in the caniuse and quirksmode datasets.
</p><p>Need to optimize with edge side includes (tell fastly to cache it as a special case) Fastly said we can do this.
</p><p>Need to work out a process for manual customization? (Maybe just the open text field?)
</p><p>Shooting for end of April to deploy on all ref pages.
</p>
<h4><span class="mw-headline" id="TOPIC:_WPD_AS_PLUGIN">TOPIC: WPD AS PLUGIN</span></h4>
<p>Tom Ortega wants to participate by investigate building plugins for standard editors: to have WPD be a plugin for these IDE. Julee referred him to frozenice as an initial contact.
</p>
<h3><span class="mw-headline" id="ACTION_ITEMS_16">ACTION ITEMS</span></h3>
<ul><li> shepazu will call in Richard Ishida, W3C's internationalization and localization expert (DONE)</li>
<li> Julee to write a draft email outlining the process to use for CSS properties review as instructions for SMEs. (DONE <a rel="nofollow" class="external free" href="http://project.webplatform.org/content/issues/43">http://project.webplatform.org/content/issues/43</a>) </li>
<li> shepazu to follow up with Lea regarding global nav (<a rel="nofollow" class="external free" href="http://project.webplatform.org/content/issues/14">http://project.webplatform.org/content/issues/14</a>) (DONE)</li>
<li> Julee to talk to ryan about this (DONE: Only GNOME project might apply. Pursuing as part of community &amp; recruiting agenda.)</li>
<li> shepazu to send out timeline for W3C GSoC (STATUS: We discussed during analytics that it probably wasn't the right)</li>
<li> Eliot &amp; shepazu to talk re: presenting at W3C WGs. (DONE: saw no follow up from julee or scottrowe. check your inboxes.)</li>
<li> shepazu to work with PPK/Verio/Alexis Deveria on public-webplatform-tests@w3.org (ON-GOING: shepazu: will report back if there's anything to report.)</li></ul>
<h2><span class="mw-headline" id="Agenda_2013-03-29">Agenda 2013-03-29</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> Status on project.*?</li>
<li> Program management meetings will be set up to:
<ul><li> Derive a final list of deliverables.</li>
<li> Get a schedule.</li>
<li> Work out how the dev/qa/launch/communication cycle will go.</li>
<li> Triage bugs.</li></ul></li>
<li> Please respond to <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Mar/0315.html">email</a> re: IRC hours and </li>
<li> Anyone want to share any status on any project?
<ul><li> Lea updated www.* with new global nav, can we get docs.* updated?</li>
<li> CSS Properties project
<ul><li> Sending out <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Mar/0308.html">emails</a> to Doc Sprint registrants to ask them to re-try getting started. Anticipating some will participate.</li>
<li> Any one else want to take on a few?</li></ul></li></ul></li>
<li> Anything blocking you from creating great content?</li>
<li> Any new or notable content to promote?</li>
<li> Julee taking a personal day next Friday. Someone willing to run this meeting?</li></ul>
<h3><span class="mw-headline" id="DISCUSSIONS">DISCUSSIONS</span></h3>
<h4><span class="mw-headline" id="TOPIC:_hiring_a_scribe">TOPIC: hiring a scribe</span></h4>
<p>shepazu proposes hiring a scribe
shepazu will report back with more information
</p>
<h4><span class="mw-headline" id="TOPIC:_CSS_properties_project_3">TOPIC: CSS properties project</span></h4>
<p>ACTION (CARRIED OVER): shepazu to recruit volunteer reviewers from the public list for CSS WG [STATUS: Prepared email. Do we have a systematic way of processing feedback? See 2013-04-12 meeting notes, above, for discussion.]
</p><p>ACTION: Julee to assign owners for properties after Doc Sprint.  (DONE)
</p><p>shepazu started work on recruiting reviewers, wrote e-mail; consulted with Fantasai
</p><p>ACTION: shepazu to send out e-mail with process/plan for tech reviewers
</p><p>We would like to get spec authors more involved with the documentation, 
with the caveat that spec authors are not the ultimate responsible party, nor should beta criteria be dependent on spec author approval
</p>
<h4><span class="mw-headline" id="TOPIC:_DOM_API_pages">TOPIC: DOM API pages</span></h4>
<p>ACTION: Content Task Force Lead [scottrowe_] should set up a meeting to talk about overall site organization and how we want to handle DOM API pages.
</p><p>scottrowe_ volunteers to be CTL for DOM API pages, julee also volunteers
</p>
<h4><span class="mw-headline" id="TOPIC:_Edit_Dismissible_Alpha">TOPIC: Edit Dismissible Alpha</span></h4>
<p>Scott's an admin, but can't change the alpha note on the main page.
</p><p>ACTION: scottrowe_ to follow up with Alex about editing the dismissible message.
</p>
<h4><span class="mw-headline" id="TOPIC:_Status_on_project..2A">TOPIC: Status on project.*</span></h4>
<p>ACTION: shepazu and julee to coordinate with garbee on project buckets, testing  (DONE)
</p>
<h4><span class="mw-headline" id="TOPIC:_Google_Summer_of_Code">TOPIC: Google Summer of Code</span></h4>
<p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:GSoC">http://docs.webplatform.org/wiki/WPD:GSoC</a>
</p><p>browser compat API in the works; maybe POC next week
</p><p>anyone can contribute to the GSoC proposal
</p><p>Shepazu - will you also be working on <a rel="nofollow" class="external free" href="http://mobilehtml5.org/">http://mobilehtml5.org/</a> to be implemented through the compat API?
</p><p>Millo, we're open to any data source that meets our criteria
</p>
<h4><span class="mw-headline" id="TOPIC:_Please_respond_to_email_re:_IRC_hours">TOPIC: Please respond to email re: IRC hours</span></h4>
<p>ACTION: If folks don't respond to email, Julee to set up an IRC calendar page  (DONE)
</p>
<h4><span class="mw-headline" id="TOPIC:_API_Project_almost_done.21">TOPIC: API Project almost done!</span></h4>
<p>Scott will send out email when it's done. 
</p>
<h4><span class="mw-headline" id="TOPIC:_Custom_error_pages.21">TOPIC: Custom error pages!</span></h4>
<p>Lea did the error pages!
</p><p><a rel="nofollow" class="external free" href="http://www.webplatform.org/errors/404.html">http://www.webplatform.org/errors/404.html</a>
</p><p><a rel="nofollow" class="external free" href="http://www.webplatform.org/errors/images/numbers.html">http://www.webplatform.org/errors/images/numbers.html</a>
</p>
<h4><span class="mw-headline" id="TOPIC:_Bug_Genie_skinning">TOPIC: Bug Genie skinning</span></h4>
<p><a rel="nofollow" class="external free" href="http://project.webplatform.org/skin/issues/3">http://project.webplatform.org/skin/issues/3</a>
</p><p><a rel="nofollow" class="external free" href="http://project.webplatform.org/prmg/issues/PRMG-10">http://project.webplatform.org/prmg/issues/PRMG-10</a>
</p>
<h3><span class="mw-headline" id="ACTION_ITEMS_17">ACTION ITEMS</span></h3>
<ul><li> (CARRIED OVER): shepazu to recruit volunteer reviewers from the public list for CSS WG (STATUS: Prepared email. Do we have a systematic way of processing feedback? See 2013-04-15 meeting notes, above, for discussion.)</li>
<li> Julee to assign owners for properties after Doc Sprint. (DONE)</li>
<li> scottrowe_ to ping jkomoros about how to fix the dismissible alpha message (DONE)</li>
<li> (CARRIED OVER): shepazu to send localization guide to public list (STATUS: Chris Mills now has this action item. Doug will bring in Richard Ishida, W3C's internationalization and localization expert)</li>
<li> Lea to implement content/issues/14 on docs.* as well (STATUS: Lea's away this week)</li>
<li> Julee set up CSS Properties project page with custom queries (Scott did this.)</li>
<li> Analytics team to develop report of key analytics, leading indicators, share at general meeting regularly (STATUS: We got the sitemap! Otherwise, carry forward)</li>
<li> shepazu to take point on next week's meeting, if there is a quorum (Meeting didn't have a quorum)</li>
<li> Content Task Force Lead [scottrowe_] should set up a meeting to talk about overall site organization and how we want to handle DOM API pages.</li>
<li> shepazu and julee to coordinate with garbee on project buckets, testing (IN PROGRESS: also programming meeting is next Wednesday)</li>
<li> If folks don't respond to email, Julee to set up an IRC calendar page <a href="/wiki/WPD:Editors_Guide/step_2_communicate_with_the_online_community#IRC_hours" title="WPD:Editors Guide/step 2 communicate with the online community">IRC hangout hours on IRC page</a> (DONE)</li></ul>
<h2><span class="mw-headline" id="Agenda_2013-03-22">Agenda 2013-03-22</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> Review <a href="/wiki/WPD:Project_Status" title="WPD:Project Status">WPD:Project_Status</a> and related <a href="/wiki/WPD:Proposals/Organizing_projects" title="WPD:Proposals/Organizing projects" class="mw-redirect">WPD:Proposals/Organizing_projects</a></li>
<li> April 3 Doc Sprint</li>
<li> Dealing with "issues". For each project, do we have:
<ul><li> A lead and team members assigned? If not, do we have volunteers?</li>
<li> Open issues assigned? If not, can we get a deadline for triaging all issues?</li></ul></li>
<li> 404 page, and other errors. - Lea volunteered to address these.</li>
<li> Anyone want to share any status on any project?
<ul><li> CSS Properties project
<ul><li> Going to CSSConf in FL in May? Do we want to plan on promoting this new content then?</li></ul></li></ul></li>
<li> Anything blocking you from creating great content?</li>
<li> Any new or notable content to promote?</li></ul>
<h3><span class="mw-headline" id="DISCUSSIONS_2">DISCUSSIONS</span></h3>
<h4><span class="mw-headline" id="TOPIC:_CSS_properties">TOPIC: CSS properties</span></h4>
<p>We will have a CSS property guide (<a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Proposals/CSS_Property_Milestone">http://docs.webplatform.org/wiki/WPD:Proposals/CSS_Property_Milestone</a>) for the upcoming doc sprint.
</p><p>The last docsprint was successful with that. There are about 160 left, and only one docsprint coming up. So we need contributors and reviewers. 
</p>
<h4><span class="mw-headline" id="TOPIC:_proposal_vs._projects_space">TOPIC: proposal vs. projects space</span></h4>
<p>Scott wants only 1 area. Does not see a difference between the two. 
</p>
<h4><span class="mw-headline" id="TOPIC:_search">TOPIC: search</span></h4>
<p>Denis needs to confirm, but we might install a new extension based on Google search (temporarily)
</p>
<h4><span class="mw-headline" id="TOPIC:_session_bug_2">TOPIC: session bug</span></h4>
<p><a rel="nofollow" class="external text" href="http://project.webplatform.org/infrastructure/issues/1">Issue #1</a> was reopened
<a rel="nofollow" class="external text" href="http://project.webplatform.org/infrastructure/issues/3">Issue #3, update error message</a> was closed
<a rel="nofollow" class="external text" href="http://project.webplatform.org/infrastructure/issues/2">Issue #2, page not refreshing</a> is not to be confused with <a rel="nofollow" class="external text" href="http://project.webplatform.org/infrastructure/issues/1">Issue #1</a>
</p><p><br />
Ryan Lane has identified this issue as an edit token issue. Excerpt from IRC of community mtg: 
</p><p>Ryan_Lane: the memcache configuration we're using now is the new style available in mediawiki since 1.18. It's what's used in production at wikimedia, and it uses the pecl memcache client, rather than mediawiki's home brewed in-php support. 
</p><p>Ryan_Lane: Are we still using the SSO plugin? And if so, do we still need it? It screws around with what's in memcache 
</p><p>patrickdsouza: if someone could look into the logs and check julee's logins you could try reproducing the bug. 
</p><p>julee: If user edits the page for a long time it is more likely to happen. 
</p><p>Ryan_Lane: Are we still using the SSO plugin? And if so, do we still need it? It screws around with what's in memcache. 
</p><p>Ryan_Lane: Are people actually logged out, or does it just say "a loss of session data" when trying to save an edit? 
</p><p>julee: I just got this error: "Oops! We seem to have a conflict. Please try saving again. If it still does not work after 2 or 3 attempts, try logging out and logging back in." I knew I was going to get that error because I had my page open in edit mode for so long 
</p><p>Ryan_Lane: that's not actually a session issue. That's an edit token issue. I'd need to see where the edit token is stored. I'd imagine memcache, but maybe not. I'm positive this could be fixed by ensuring logged in users always hit the same application server once they are logged in, but that's really just avoiding the real problem 
</p>
<h4><span class="mw-headline" id="TOPIC:_4.2F3_Doc_Sprint">TOPIC: 4/3 Doc Sprint</span></h4>
<p>Peter already has secured facilities and catering. It's at Google's offices in SFL:
</p>
<ul><li> very much like previous doc sprints</li>
<li> the big ticket item this time is CSS properties project, but other people should suggest other projects</li>
<li> Scott to run new people through a getting started observe whether the getting started pages/workflow is working for people. 4 or 5 people .</li>
<li> So many Doc Sprints in the Bay Area. We might really want to try to incorporate remote participation again.</li>
<li> It starts at 9, but you can come early. I'll be there by 8, 8:30.</li>
<li> We'll have schwag, a bunch of t-shirts</li></ul>
<h4><span class="mw-headline" id="TOPIC:_Dom_API">TOPIC: Dom API</span></h4>
<p>A quick huddle to talk about overall site organization and how we want to handle DOM API pages. There are multiple ways to look at DOM. We want to entertain different viewpoints into the model, based on the way people experience it. We're not locked into a single hierarchy because this isn't a book. Only one URL structure, but maybe multiple views?
</p><p>We may begin talk at Doc Sprint or Content project area lead will set a meeting to discuss.
</p>
<h4><span class="mw-headline" id="TOPIC:_Dealing_with_.22issues.22">TOPIC: Dealing with "issues"</span></h4>
<p>A bunch of issues are sitting around. Let's get project owners and encourage triage and status on bugs, at the project level. Then these projects roll up in some way in summary.
</p><p>Minimally, we should get all issues in bug genie assigned (something that bugzilla requires).
</p>
<h4><span class="mw-headline" id="TOPIC:_404_page">TOPIC: 404 page</span></h4>
<p>Lea agreed to look into the UX for 404 pages. She will design and will request fine tuning of content. 
<a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Projects/ErrorPages">http://docs.webplatform.org/wiki/WPD:Projects/ErrorPages</a>
</p>
<h4><span class="mw-headline" id="TOPIC:_Code_styles">TOPIC: Code styles</span></h4>
<p>shepazu hid code markup styling because it were ugly, but leaverou restyled and brought back. She added Prism.js. Before, the code examples had an indication of what language they were in, but the markup wasn't in the format prism expected. So, leaverou wrote some code to transform to the right format, so we now have nicely highlighted ones! It only works on samples with a language set.
</p>
<h4><span class="mw-headline" id="TOPIC:_Global_navs">TOPIC: Global navs</span></h4>
<p>leaverou implemented the bottom global content navs! She is also willing to take up <a rel="nofollow" class="external text" href="http://project.webplatform.org/content/issues/14">Issue #14</a>: 
</p>
<h3><span class="mw-headline" id="ACTION_ITEMS_18">ACTION ITEMS</span></h3>
<p>ACTION (CARRIED OVER): EVERYONE:
</p>
<ul><li> if you haven't been editing pages, can you volunteer to do a CSS property? that will get you used to editing the wiki and experiencing what our users are experiencing?</li>
<li> also try to recruit one or two people to do some property pages.</li>
<li> and if you could help me with the review process. If there are certain pages that should be reviewed by an expert, call them out to me.</li>
<li> and if you have ideas of experts who would be good reviewers, let me know--we need a significant number of them before we can claim that the docs are good</li>
<li> Use the new "needs review" tag to tag articles that need review</li></ul>
<p>ACTION (CARRIED OVER): shepazu to recruit volunteer reviewers from the public list for CSS WG
</p><p>ACTION (CARRIED OVER): shepazu to send localization guide to public list
</p><p>ACTION (CARRIED OVER): Julee to call it out to the l18n folks to make sure it makes sense &amp; add it to the Ed-Guide.  (Shepazu wants Richard I to be involved.)
</p><p>ACTION: scottrowe, update the Proposals section to be Projects [DONE]
</p><p>ACTION: Julee to send out Beta Plan decision to public list [DONE]
</p><p>ACTION: Lea to implement content/issues/14
</p><p>ACTION: Julee to update issue with URL that new links should point to. [DONE]
</p><p>ACTION: Content Task Force Lead [TBD] should set up a meeting to talk about overall site organization and how we want to handle DOM API pages. 
</p><p>ACTION: Julee to send out e-mail asking for a lead, at least temporarily, for each project area, so we can get bug triaged and some movement. [DONE]
</p>
<h2><span class="mw-headline" id="Agenda_2013-03-15">Agenda 2013-03-15</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> <a rel="nofollow" class="external text" href="http://docs.webplatform.org/wiki/WPD:Tasks/CSS_Property_Milestone">CSS Properties project</a>
<ul><li> Volunteer to get pages written.</li>
<li> Send Julee your recommendation for props that really should be reviewed &amp; suggested experts.</li>
<li> Pointer to APIs.</li></ul></li>
<li> Topic vs. Topic Clusters?</li>
<li> Filling out the taxonomy of the site 
<ul><li> Generate a site map of the current site</li>
<li> Identify what pages should be there that aren't</li>
<li> Stub in those pages with details on priority, etc.</li></ul></li>
<li> URLs for translation
<ul><li> What can we tell translators now?
<ul><li> Why can't we do ..wiki/lang/.. now?</li></ul></li>
<li> Should we have a task force?</li></ul></li>
<li> Fix Search
<ul><li> Duplicate pages in results</li>
<li> Crawl/index WPD: pages for help</li></ul></li>
<li> Session bug?</li>
<li> Dabblet?</li>
<li> Community development task force
<ul><li> Press kit?
<ul><li> Brief recap of <a href="/wiki/WPD:Community/Survey/Verbatims" title="WPD:Community/Survey/Verbatims">Verbatims</a> and <a href="/wiki/WPD:Community/Survey/Doc_Sprint/Berlin_2-2013" title="WPD:Community/Survey/Doc Sprint/Berlin 2-2013">Survey</a>.</li>
<li> Plan next Doc Sprint: April 3, 2013 in San Francisco at the Google office.</li></ul></li></ul></li>
<li> Analytics task force
<ul><li> Getting together in the next week</li></ul></li>
<li> Content-complete questions:
<ul><li> How can we get a seal of approval from the community? Can SME review content?</li>
<li> What is the criteria for calling something complete?</li>
<li> What is the announcement plan to promote completed content?</li></ul></li>
<li> Anything blocking you from creating great content?</li>
<li> Any new or notable content to promote?</li></ul>
<h3><span class="mw-headline" id="Discussion_16">Discussion</span></h3>
<h4><span class="mw-headline" id="TOPIC:_CSS_Properties_2">TOPIC: CSS Properties</span></h4>
<p>ACTION: * everyone:
</p>
<ul><li><ul><li> if you haven't been editing pages, can you volunteer to do a CSS property? that will get you used to editing the wiki and experiencing what our users are experiencing?</li>
<li> also try to recruit one or two people to do some property pages.</li>
<li> and if you could help me with the review process. If there are certain pages that should be reviewed by an expert, call them out to me.</li>
<li> and if you have ideas of experts who would be good reviewers, let me know--we need a significant number of them before we can claim that the docs are good</li>
<li> Use the new "needs review" tag to tag articles that need review</li></ul></li></ul>
<p>ACTION: shepazu to reach out to public CSS WG list and ask for experts to review CSS pages
</p><p>For the beginning, the webkit team will likely just need a stable URL scheme and that's it, so they can generate lists
</p><p>Eliot said that, unfortunately, someone who was going to join the project won't be able to join due to personal reasons. looking for someone to take his place, but no great options at the moment
</p>
<h4><span class="mw-headline" id="TOPIC:_Topic_vs_Topic_Clusters">TOPIC: Topic vs Topic Clusters</span></h4>
<p>scottrowe_ did docs on that. more usable and better-accessed during the getting started flow and editor's guide
</p>
<h4><span class="mw-headline" id="TOPIC:_Taxonomy_of_the_site">TOPIC: Taxonomy of the site</span></h4>
<p>We still want to generate a sitemap. Doug and I spoke about this over e-mail to the list. Doug is going to get Julee access so she can experiment with generating a sitemap.
</p><p>ACTION: Denis to follow up with Julee about sitemap generation [DONE]
</p><p>scottrowe_ has been looking into the DOM project in relation to the Shadow DOM documentation. He's trying to figure out how we should design our DOM API pages generally. He will propose the DOM project as next quarter's project, just like CSS was this quarter's project.
</p><p>Let's focus on CSS properties first.
</p><p>DOM organization &amp; refactoring is a pre-beta criteria. Even if we could just settle how we're going to organize it, then we could have a solid beta presentation.
</p><p>Coming up with a set of beta guidelines soon. It will include the DOM is part of the architecture of the site is a pre-beta criteria
</p><p>Segment the site (E.g. css properties) getting to "beta" individually as their quality gets to the right level.
</p><p>But make it clear what's beta and what isn't. Add visual cues to each section so the solid stuff looks solid, and placeholders look partly there.
</p><p>And map out what ALL of the pages are and creating stubs. And that goes along with the sitemap that Julee's working on. And helps us not have to explain the new page flow to new contributors – they'll be pre-populated.
</p><p>This conference is full, no more parties can be added.
</p><p>ACTION: Shepazu to allocate more spaces in future calls
</p>
<h4><span class="mw-headline" id="TOPIC:_URLs_for_translation">TOPIC: URLs for translation</span></h4>
<p>Some concern over current URL naming schema. We have a page that writes up how to do this. It's not a great process, but it is possible. 
</p><p>We should do one or more BoF sessions at the html5devcon, to generate buzz, invite folks to grapple with how to handle i18n, catch folks who can't make the sprint, help pack the sprint, etc.
</p><p>We should address this now if we have volunteers who want to help out. 
</p><p>ACTION: Shepazu to get richard ishia [sp?] comment on what a better solution will be. He's the W3C l18n expert
</p><p>The localization guide isn;'t in the editor's guide.
</p><p>ACTION: shepazu to send localization guide to public lis
ACTION: Julee to call it out to the l18n folks to make sure it makes sense (shepazu wanted to get Richard I involved...)
</p><p>We will table the long-term solution for now
</p>
<h4><span class="mw-headline" id="TOPIC:_Search_2">TOPIC: Search</span></h4>
<p>Why we can't fix this part with duplicate results? the default search is bad for mediawiki. We thought we replaced it with Lucene.
With the advanced search you can already include WPD pages
</p><p>ACTION: Denis and shepazu to talk about improving built-in search. (Did we replace default search with Lucene?) (Lea to shepazu: this might help: <a class="external free" href="http://www.mediawiki.org/wiki/Extension:SphinxSearch">http://www.mediawiki.org/wiki/Extension:SphinxSearch</a>)
</p>
<h4><span class="mw-headline" id="TOPIC:_Session_bug_status">TOPIC: Session bug status</span></h4>
<p>Feedback from users: it's still happening.
</p><p>Denis talked to fastly guys two weeks ago. He said to change something in the config of servers. But it must not have worked.
</p><p>ACTION: Denis to continue debugging the session bug
</p>
<h4><span class="mw-headline" id="TOPIC:_Taskforces">TOPIC: Taskforces</span></h4>
<p>Do we want to report status here, or just in project.webplatform.org?
</p><p>We can subscribe to updates from task forces via project.webplatform.org
</p><p>Also, cover highlights from the task teams in this weekly meeting.
</p>
<h5><span class="mw-headline" id="SUBTOPIC:_Community_development_task_force">SUBTOPIC: Community development task force</span></h5>
<p>Not enough data from Feb 23rd DocSprint. Next DocSprint 4/3 around HTML5DevConf. They have on their conference webpage they have a signup for WPD. They have about 35 people signed up through EventBrite for conference website, and we have 70 or so on our site. 
</p><p>Sync community TF goals with project planning.
</p><p>ACTION: scottrowe_ to set up meeting about next doc sprint
</p><p>There are young CS students who are interested in getting involved in community.
</p><p>We are planning to have doc sprints on the east coast. One in Ohio this summer, and at least 2 doc sprints in NC (one in summer, one in fall) – NYC has been requested.
</p>
<h5><span class="mw-headline" id="SUBTOPIC:_Analytics_task_force">SUBTOPIC: Analytics task force</span></h5>
<p>We're having our first meeting this week.
</p>
<h4><span class="mw-headline" id="TOPIC:_Content_completeness">TOPIC: Content completeness</span></h4>
<p>Now that we have project.webplatform.org, we'll build it into the workflow.
</p><p>Promotion: Blog posts for even small new additions are great, but for big milestones, we should have more press outreach
</p><p>ACTION: julee to follow up with garbee on how to do workflows and forms in BG  (DONE)
</p><p>We talked yesterday about figuring out fields and milestones. Garbee has promised to document things about BG and has committed to do some videos. We may want to set up another session for other people.
</p>
<h4><span class="mw-headline" id="TOPIC:_Any_new_or_notable_content_to_promote.3F">TOPIC: Any new or notable content to promote?</span></h4>
<p>Adobe gave us some of Mike Sierra's times. He created several articles, one on transforms that's quite good. He's currently working on SVG
I think that's notable and good to share. We've shared some of it and got a bunch of retweets. We should be more aggressive about tweeting out new batches of articles that we've created.
</p><p>Also, for the last 6 months we've benefited from the participation of Dave Gash, a contractor at Google, worked on API pages and CSS properties. There are a handful more to do, then we should put together a comm plan for that content.
</p><p>ACTION: shepazu to invite people to twitter account
</p><p>Remember it's good to get a quick LGTM from someone in IRC for spelling, links, etc.
</p><p>ACTION: peterlubbers to invite people to the Google+ admins
</p><p>Folks are putting bylines on articles. That's appropriate for primary authors. It's a nice incentive.
</p><p>perhaps we should have a clearer policy around author attribution or have a significant contributions page to highlight contributions? It's capture din MediaWiki, but not highlighted well.
</p><p>publicity workflow -- it should be easy to rain kudos on a team member when they earn it
</p><p>mozilla blog they have open badges 1.0 <a rel="nofollow" class="external free" href="https://blog.mozilla.org/blog/2013/03/14/open_badges/">https://blog.mozilla.org/blog/2013/03/14/open_badges/</a>
</p><p><br />
ACTION: Julee to add comm plan as a topic for the community taskforce. (DONE)
</p>
<h4><span class="mw-headline" id="TOPIC:_Kuma">TOPIC: Kuma</span></h4>
<p>Denis has been reviewing Kuma, made a local installation. So far, it's been easy to install. But he needs to figure out if it can be a good fit. Janet sent Denis some contacts, Kuma developers. They've been very helpful. This is background stuff, shouldn't affect any work going on. 
</p>
<h3><span class="mw-headline" id="Actions">Actions</span></h3>
<ul><li> Denis to follow up with Julee about sitemap generation [DONE]</li>
<li> Shepazu to allocate more spaces in future community meeting calls [DONE]</li>
<li> Shepazu to get richard ishia [sp?] comment on what a better solution will be. He's the W3C l18n expert [DEFERRED]</li>
<li> Denis and shepazu to talk about improving built-in search. [Denis is working on this.]</li>
<li> Denis to continue debugging the session bug [Denis is working on this.]</li>
<li> scottrowe_ to set up meeting about next doc sprint [DONE – this meeting&#160;;-) ]</li>
<li> julee to follow up with garbee on how to do workflows and forms in BG [Garbee is working on this.]</li>
<li> shepazu to invite people to twitter account  [DONE]</li>
<li> peterlubbers to invite people to the Google+ admins  [DONE]</li>
<li> Julee to add comm plan as a topic for the community taskforce  [DONE]</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="Agenda_2013-03-08">Agenda 2013-03-08</span></h2>
<p>Meeting adjourned for lack of a quorum.
</p>
<h2><span class="mw-headline" id="Agenda_2013-03-01">Agenda 2013-03-01</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> <a rel="nofollow" class="external text" href="http://docs.webplatform.org/wiki/WPD:Tasks/CSS_Property_Milestone">CSS Properties project</a>
<ul><li> What are the next steps for this project?</li></ul></li>
<li> DocSprints
<ul><li> How was w3cconf DocSprint @ Adobe?</li>
<li> Next DocSprint?</li></ul></li>
<li> Session bug status?</li>
<li> Bug Genie status?</li>
<li> Dabblet status?</li>
<li> template for the native JS objects?</li>
<li> New task forces
<ul><li> Communications and recruiting</li>
<li> Analytics</li>
<li> Reporting back to this meeting?</li></ul></li>
<li> Anything blocking you from creating great content?</li>
<li> Any new or notable content to promote?</li></ul>
<h3><span class="mw-headline" id="Doc_Sprints">Doc Sprints</span></h3>
<p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Community/Community_Events">http://docs.webplatform.org/wiki/WPD:Community/Community_Events</a>
</p>
<ul><li> 2/23 DocSprint: attendance: 27; CSS Properties worked on: 23</li>
<li> Possibility of next Docsprint at HTML5DevConf - Mid-April</li>
<li> Possible Docsprint in Puget Sound Area Mid-April</li>
<li> <a rel="nofollow" class="external free" href="http://openhelpconference.com/">http://openhelpconference.com/</a></li></ul>
<p><br />
</p>
<h3><span class="mw-headline" id="Action_items_19">Action items</span></h3>
<ul><li> JULEE will work on getting a burndown together [DONE]</li>
<li> Julee - Setup Analytics project at project.webplatform.org [DONE]</li>
<li> Eliot: Follow up on getting documentation into Editing Guidelines for using codelet at DocSprints to do code examples [DONE] [<a rel="nofollow" class="external autonumber" href="http://docs.webplatform.org/wiki/WPD:Manual_Of_Style/Sample_best_practices">[1]</a>]</li>
<li> Julee to add agenda item for next week: Topic vs. Topic Clusters [DONE]</li>
<li> Julee to add agenda item for next week: Getting SME to review content [DONE]</li></ul>
<h2><span class="mw-headline" id="Agenda_2013-02-15">Agenda 2013-02-15</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> <a rel="nofollow" class="external text" href="http://docs.webplatform.org/wiki/WPD:Tasks/CSS_Property_Milestone">CSS Properties status</a>
<ul><li> How did the testing go? Were folks able to create property pages?</li>
<li> Do we want to do some sort of review? How?</li>
<li> How shall we divy up the remaining properties?</li>
<li> What are the next steps for this project?</li></ul></li>
<li> w3cconf DocSprint @ Adobe
<ul><li> Who's going? (Shepazu, Craig, Eliot, Julee maybe Peter)</li>
<li> What should we focus on?</li></ul></li>
<li> Session bug status?</li>
<li> Bug Genie</li>
<li> Webplatform preso for w3cconf</li>
<li> Anything blocking you from creating great content?</li>
<li> Any new or notable content to promote?</li></ul>
<h3><span class="mw-headline" id="Summary">Summary</span></h3>
<h4><span class="mw-headline" id="CARRIED_OVER_FROM_LAST_WEEK">CARRIED OVER FROM LAST WEEK</span></h4>
<p>1. ACTION (carried forward): shepazu + denis to implement sitemap extension
</p>
<ul><li> Carried forward again</li></ul>
<p>2. ACTION (carried forward): Alex to sort out updating the CSS properties template to reflect Mike S's Gold standard CSS property page
</p>
<ul><li> Carried forward again</li></ul>
<p>3. ACTION (carried forward): others should try to implement a CSS property page, and use chrismills' instructions when they are finished
</p>
<ul><li> Finished</li></ul>
<p>4. ACTION (carried forward): determine a set of properties we know to be complex outliers
</p>
<ul><li> Finished</li></ul>
<p>5. ACTION: JULEE to send out email to public list to get input regarding spec status  (DONE)
</p>
<ul><li> Finished</li></ul>
<p>6. ACTION: Shepazu to investigate cloud infrastructure and latency as possible roots of session bug
</p>
<ul><li> Investigated with help from HP Cloud people, no resolution as yet. Ongoing.</li></ul>
<p>7. ACTION: chrismills: recruit more participants to css properties project, augmenting tracking spreadsheet, actively tracking progress
</p>
<ul><li> Ongoing. Has invited one person to take part (Rachel Andrew), who agreed to help out.</li></ul>
<h4><span class="mw-headline" id="NEW_ACTIONS_FOR_THIS_WEEK">NEW ACTIONS FOR THIS WEEK</span></h4>
<ul><li> ACTION: chrismills, make google spreadsheet just show p0-p2, css properties</li>
<li> ACTION: chrismills: pull together 10-15 good CSS example pages and mail them around. People from different companies will then send these example pages to their resident CSS spec gurus, e.g Tab Atkins, Fantasai, Howcome, etc. and see what they think, as well as real world CSS gurus, e.g. Rachel Andrew, Chris Coyier, Peter Gasston, Dan Cederholm, Ethan Marcotte, Nicole Sullivan (their needs will be different.)</li>
<li> ACTION: all, give Doug suggestions on what to add to WPD session him and Janet are doing at W3Conf</li>
<li> ACTION: Scott to spruce up the APIs landing page</li></ul>
<h2><span class="mw-headline" id="Agenda_2013-02-01">Agenda 2013-02-01</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> <a rel="nofollow" class="external text" href="http://docs.webplatform.org/wiki/WPD:Tasks/CSS_Property_Milestone">CSS Properties status</a>
<ul><li> Exemplar and instructions are completed; 5 folks are testing the workflow.</li>
<li> <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/buglist.cgi?query_format=specific&amp;order=relevance%20desc&amp;bug_status=__open__&amp;product=webplatform.org&amp;content=session&amp;list_id=4654">Session bug</a> was a blocker. Ryan tried to resolve the issue. Observations?</li>
<li> Spec status values should be resolved. Lea brings up a good point: maybe we should be calling it "browser support". <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=20386">20386</a> <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=18896">18896</a></li></ul></li>
<li> Dealing with browser compat info — it is hard and time consuming; can we automate it? See mail from Doug May: <a rel="nofollow" class="external free" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Feb/0002.html">http://lists.w3.org/Archives/Public/public-webplatform/2013Feb/0002.html</a>. See also: <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Compatibility_Info">http://docs.webplatform.org/wiki/WPD:Compatibility_Info</a></li>
<li> Analytics?</li>
<li> Attracting contributors:
<ul><li> Session bug needs resolving</li>
<li> Getting started experience validated via usability study @ DocSprint Berlin</li>
<li> Communications on blogs picking up</li>
<li> Additional plans?</li></ul></li>
<li> Anything blocking you from creating great content?</li>
<li> Any new or notable content to promote? Does someone want to write up a blog post for Web Audio API?</li></ul>
<h3><span class="mw-headline" id="Topics">Topics</span></h3>
<ul><li> TOPIC: CSS Properties project status
<ul><li> SUBTOPIC: spec status value on exemplar page.
<ul><li> <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/css/properties/font-size">http://docs.webplatform.org/wiki/css/properties/font-size</a></li>
<li> <a rel="nofollow" class="external free" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=20386">https://www.w3.org/Bugs/Public/show_bug.cgi?id=20386</a></li>
<li> font-style property page spec status: values are not usable; bug filed; considering different values than those of W3C</li>
<li> How to represent feature status so visitor knows whether it's in most browsers? Production-ready?</li>
<li> Community does need to know the status so it can participate. Need to bring the community in the standard development process; need to know if a spec is in "last call" or what, so the community can know whether/how to participate.</li>
<li> Should we add information about level of usability? Providing both values? Should we move this info to the bottom of the page? Near compatibility? Or should it stay up top for easy identification? Maybe an easy flag up top with details below?</li>
<li> html5please.com was offered up as a site that does it well: <a rel="nofollow" class="external free" href="http://html5please.com/#gradients">http://html5please.com/#gradients</a></li></ul></li>
<li> ACTION: JULEE to send out email to public list to get input.</li>
<li> SUBTOPIC: The dreaded SESSION BUG!!! (Bug#19914). Memcache fix does not appear to solve the problem. It might be cloud infrastructure issue.</li>
<li> ACTION: Shepazu to investigate cloud infrastructure and latency</li>
<li> SUBTOPIC: recruiting participants for CSS properties project
<ul><li> ACTION: cmills: recruit more participants to css properties project, augmenting tracking spreadsheet, actively tracking progress</li></ul></li></ul></li>
<li> TOPIC: Doug May has a way of dealing with browser compat info — it is hard and time consuming; can we automate it? See mail from Doug May: <a rel="nofollow" class="external free" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Feb/0002.html">http://lists.w3.org/Archives/Public/public-webplatform/2013Feb/0002.html</a>. See also: <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Compatibility_Info">http://docs.webplatform.org/wiki/WPD:Compatibility_Info</a>
<ul><li> shepazu: idea: to update compat from different sources: quirksmode, caniuse, w3c test suites/test the web forward and auto-generate from that</li>
<li> Doug May is investigating data-tree based solution to assess the suitability of data point, then refine algorithm for data retrieval that includes human-intervention provision.</li></ul></li>
<li> ACTION: Doug May and Chris to collaborate on solution in Berlin, and hopefully define a solution for SF doc sprint.</li>
<li> TOPIC: Analytics?
<ul><li> What is the current status of work on analytics? Site traffic, usage, etc.</li></ul></li></ul>
<p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/Special:Statistics">http://docs.webplatform.org/wiki/Special:Statistics</a>
</p>
<ul><li> ACTION: Julee to call for participation/leadership on e-mail. [DONE]</li>
<li> TOPIC: Recruiting experts and editors.
<ul><li> Cmills is working on recruiting CSS experts, get them to contribute.</li></ul></li>
<li> ACTION: cmills: to contact university lecturers on garnering participation of college students.
<ul><li> shepazu: maybe we could do college campus doc sprints</li>
<li> shepazu: wary of unleashing this ahead of site estabilshment, Julee seconds</li>
<li> Craig: need to improve the Getting Started workflows, </li></ul></li></ul>
<p>need to identify content areas of priority, focus on areas that provide sense of satisfaction
</p>
<ul><li><ul><li> shepazu: would like to prioritize blog posts around content that is usable, current</li>
<li> shepazu: use the blog software to draft, instead of e-mails</li></ul></li>
<li> Motion to establish a working group to investigate, develop communications plan</li>
<li> ACTION: Scott to focus survey on doc sprints</li>
<li> ACTION: Julee: to mail calling for participation in communication/outreach working group  (DONE)</li>
<li> ACTION: Eliot to start off-line thread around blog posting priorities, suitability</li>
<li> TOPIC: New and notable activities on WPD?
<ul><li> <a rel="nofollow" class="external free" href="https://github.com/webplatform/Shortlinks">https://github.com/webplatform/Shortlinks</a> - fr0zenice's shortlinks system for WPD</li></ul></li></ul>
<p><br />
</p>
<h3><span class="mw-headline" id="ACTIONS_2">ACTIONS</span></h3>
<ul><li> ACTION (carried forward): shepazu + denis to implement sitemap extension: Concerns about current solution viability; looking for alternate. </li>
<li> ACTION (carried forward): julee and garbee to look into installing meetbot: Garbee to try to work on it more on the weekend.  (DONE)</li>
<li> ACTION (carried forward): Alex to sort out updating the CSS properties template to reflect Mike S's Gold standard CSS property page: IN PROGRESS, Alex to consult w frozenice on scope.</li>
<li> ACTION (carried forward): others should try to implement a CSS property page, and use chrismills' instructions when they are finished: IN PROGRESS</li>
<li> ACTION (carried forward): determine a set of properties we know to be complex outliers: in progress</li></ul>
<ul><li> ACTION: JULEE to send out email to public list to get input regarding spec status  (DONE)</li>
<li> ACTION: Shepazu to investigate cloud infrastructure and latency as possible roots of session bug</li>
<li> ACTION: cmills: recruit more participants to css properties project, augmenting tracking spreadsheet, actively tracking progress</li></ul>
<p><br />
</p>
<h4><span class="mw-headline" id="Completed_Actions">Completed Actions</span></h4>
<ul><li> ACTION (carried forward): eliot to edit top level landing pages:DONE</li>
<li> ACTION: Mike S to move his static font-size example into the appropriate Wiki page:DONE</li>
<li> ACTION: Chris to finish writing a guide to implementing a CSS properties page:DONE</li>
<li> ACTION: Mike to work out how to specify "dependant/dependency properties":DONE</li>
<li> ACTION: Scott to add an instruction in the attribution template that says "hey - don't delete this or change this unless you have a really good reason":DONE</li>
<li> ACTION: Doug, Denis, Lea, work on implementing first phase of Dabblet live coding examples:DONE</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="Agenda_2013-01-25">Agenda 2013-01-25</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> <a rel="nofollow" class="external text" href="http://docs.webplatform.org/wiki/WPD:Tasks/CSS_Property_Milestone">CSS Properties milestones</a>
<ul><li> Pick a few for folks to try out using Mike's example.</li>
<li> Any volunteer to write up instructions based on Mike's gold standard?</li></ul></li>
<li> Attributions</li>
<li> Status on code.webplatform.org?</li>
<li> Moving from MediaWiki</li>
<li> Status on "discoverability" <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=19401">Search Bug</a>
<ul><li> Do we have an interim solution we can implement quickly &amp; easily</li>
<li> We're going to put a search box on the <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=19694">main page</a></li></ul></li>
<li> Analytics</li>
<li> Anything blocking you from creating great content?</li>
<li> Any new or notable content to promote?</li></ul>
<h3><span class="mw-headline" id="Actions_3">Actions</span></h3>
<ul><li> ACTION: shepazu + denis to implement sitemap extension</li>
<li> ACTION (carried forward): eliot to edit top level landing pages [DONE]</li>
<li> ACTION (carried forward): julee and garbee to look into installing meetbot  (DONE)</li>
<li> ACTION: Alex to sort out updating the CSS properties template to reflect Mike S's Gold standard CSS property page</li>
<li> ACTION: Mike S to move his static font-size example into the appropriate Wiki page</li>
<li> ACTION: Chris to finish writing a guide to implementing a CSS properties page</li>
<li> ACTION: others should try to implement a CSS property page, and use chrismills' instructions when they are finished</li>
<li> ACTION: determine a set of properties we know to be complex outliers, and make sure they fit with Mike's scheme, for example background-image (with radial gradient, linear gradient, etc) perspective transforms with multiple values set (crazy: transforms take any # of functions &amp; assume defaults; "filter" prop takes functions in sequence) properties that don't have any effect unless another property is set. So for example, top, left, bottom, right don't have any effect unless you already set position: relative or position: absolute, flex and order do not have an effect unless display: flex is set properties that are proprietary and are only ever used with -ms- or -webkit-, for example</li>
<li> ACTION: Mike to work out how to specify "dependant/dependency properties"</li>
<li> ACTION: Scott to add an instruction in the attribution template that says "hey - don't delete this or change this unless you have a really good reason"</li>
<li> ACTION: Doug, Denis, Lea, work on implementing first phase of Dabblet live coding examples</li>
<li> ACTION: Doug to get together a task force to continue investigating an alternative to MW for our platform</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="Agenda_2013-01-17">Agenda 2013-01-17</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> Status on code.webplatform.org?</li>
<li> <a rel="nofollow" class="external text" href="http://docs.webplatform.org/wiki/WPD:Proposals/api_docs">Scott's API proposal</a> (<a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2013Jan/0069.html">See thread.</a>)</li>
<li> <a rel="nofollow" class="external text" href="http://docs.webplatform.org/wiki/WPD:Tasks/CSS_Property_Milestone">CSS Properties milestones</a>.</li>
<li> Status from Chris Mills: "I made loads of progress on filling in  the master CSS properties list today, building on top of Alex's great work. I'll try to finish this list tomorrow."</li>
<li> Status on "discoverability"
<ul><li> <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=19401">Search</a>
<ul><li> Do we have an interim solution we can implement quickly &amp; easily</li>
<li> We're going to put a search box on the <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=19694">main page</a></li></ul></li>
<li> Global nav</li>
<li> In-context ToCs</li></ul></li>
<li> Anything blocking you from creating great content?</li>
<li> Any new or notable content to promote?</li>
<li> Need a new time for this meeting?</li></ul>
<h3><span class="mw-headline" id="Meeting_Summary">Meeting Summary</span></h3>
<ul><li> Several folks weren't available to discuss open issues and action items. </li>
<li> We talked about a Table of Contents or nav at the top of articles. There was a TOC in the skin, and also one based on a user preference. They conflicted, so we took it out of the skin but if no users have set the preference to show it, we could bring the skin TOC back. But the default ToC was ever styled since</li></ul>
<p>someone had a plugin they wanted to use.
</p>
<ul><li> We are planning blog posts on Audio API and CSS regions</li>
<li> Janet is going to FOSDEM. Anyone else?</li>
<li> CSS properties proposal: about 2/3 thru prioritization of properties. Goal is to finish tomorrow, and work on a "representative" article. Then we need to create an author's guide based on the representative article. The property worked on previously was 'font-size'. Mike Sierra to work on making a "gold standard" example page, that others can use as a model. <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/css/properties/font-size">http://docs.webplatform.org/wiki/css/properties/font-size</a></li></ul>
<h3><span class="mw-headline" id="Actions_4">Actions</span></h3>
<p>ACTION: Julee to send out a Doodle poll to figure out a better time. [Done]
ACTION: Mike Sierra to work on making a "gold standard" example page, that others can use as a model. [DONE]
LAST WEEK ACTION: Julee to update Topic Hierarchy and Architecture pages. UPDATE: need site map
LAST WEEK ACTION: Eliot to do an editorial pass on the proposed top-level pages. [DONE]
LAST WEEK ACTION: Julee to set up meetbot. UPDATE: Garbee now has action item.  (DONE)
</p>
<h2><span class="mw-headline" id="Agenda_2013-01-10">Agenda 2013-01-10</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> Triage of new content architecture issues
<ul><li> All <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/buglist.cgi?product=webplatform.org&amp;component=content&amp;resolution=---&amp;list_id=2513">content bugs</a> are assigned to either Chris or Garbee. Do we want to re-assign some of them?</li></ul></li>
<li> Status on <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=20160">bug#20160</a></li>
<li> Current workflow for promoting new/great content? (Propose, Review, Sign-off?)</li>
<li> DocSprint in Germany
<ul><li> Anyone going?</li>
<li> Registration for the first european Doc Sprint in Berlin, Feb 8+9 2013, is now open. Please help to spread the word:
<ul><li> <a rel="nofollow" class="external text" href="https://plus.google.com/100575683580946332118/posts/iLxwzGU6zac">Share</a></li>
<li> <a rel="nofollow" class="external text" href="https://alpha.app.net/klick_ass/post/2113801">Repost</a></li>
<li> <a rel="nofollow" class="external text" href="https://twitter.com/klick_ass/status/281775907734167553">Retweet</a></li></ul></li></ul></li>
<li> Scott is working on Listing pages (Per Scott's email Thursday, December 20, 2012 11:35 AM; Subject: Re: New topic landing pages installed (was Re: We have a new front page))</li>
<li> Status on Dabblet?</li>
<li> Anything blocking you from creating great content?</li></ul>
<h2><span class="mw-headline" id="Meeting_Summary_2">Meeting Summary</span></h2>
<h3><span class="mw-headline" id="Discussion_17">Discussion</span></h3>
<ul><li> We're adding an API section to the topic landing pages. We need to include APIs and their icons on those pages. Seb is working on an icon, and Chris will put that in the landing page</li>
<li> Concept_Listing template is done</li>
<li> Continuing to work on API area: reorganizing it and following through on previous work we've done. The APIs section is starting to come around, with help from Dave Gash.</li>
<li> Promoting new or great content. To post about WPD topics, see  <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Marketing/Posting_Guidelines">http://docs.webplatform.org/wiki/WPD:Marketing/Posting_Guidelines</a>. 
<ul><li> The process right now is shoot it into the Mailing List, wait a bit, and see if anyone disagrees with it. Doug will set up additional bloggers. This content task force will continue to request suggestions for "Any new and notable content to promote"</li></ul></li>
<li> DocSprint Germany: Scott Rowe is probably going.</li>
<li> We received status on the Dabblet extensions. The consensus on the list was code.webplatform.org. Lea has put the technical things in place in her codebase there's still some work to do to link from. First is a dabbler instance on code.webplatform.org. The second phase is to make it easy to open examples on the site in that instance (a "try now" button). Third phase is actual live code examples in the pages themselves. (possibly) via iframes. (There's actually a phase 4 that allows us to decouple a dependency on github.) We're aiming to have first phase done by next week. And we should have a blog post about it. We also need to get a template made with the form to submit/change code in the forms. Garbee is emailing Tomato this afternoon to see if she would be up for that. </li>
<li> We need more work on getting started pages (bug&#160;: <a rel="nofollow" class="external free" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=20160">https://www.w3.org/Bugs/Public/show_bug.cgi?id=20160</a>). At last doc sprint was they just can't get through them -- somewhere between five and ten people. When we walked them through the basics, they had a hard time getting productive. Following through the instructions is difficult. It should be more self-serve. Julee to send outline of new Editor's Guide next week. Scott to work on usability testing. Also, there are going to be some people who don't respond to the given way. So maybe we have other docs for different mind sets. Scott and Peter are working on Getting Started videos. 
<ul><li> Additional Getting Started problems: 
<ul><li> The form system. For example, we've seen people wanting to use API_Listing template on other pages, which breaks pages (it uses two forms).</li>
<li> There was a glitch in the process for updating compatibility tables. A lot of the pages in the "Pages that need compatibility table" weren't working.</li>
<li> A lot of people at the Sprint were confused with them. I actually spent most of the day there explaining it to people.</li>
<li> A handful actually went to editing source because the button was there. Some of us want to remove that button unless you are an admin or in the template corp group whenever that gets made.</li>
<li> Besides forms people were getting hit hard by the template bugs that require the hacks like | and =. We need to either fix it so those hacks aren't required or look at another way of doing things.</li></ul></li>
<li> Additional solutions:
<ul><li> One way to fix the hacks would be editing as much as possible in raw HTML. Leaving mostly only links to be made in the wiki markup.</li>
<li> Garbee has an open bug report for it iirc. Has been there for a while. I will bring attention to it once we get an in-house system going.</li>
<li> People also seemed to be lost in what was needed to be done. We should try to use the content tracker to a greater extent once we get it in-house.</li>
<li> Another way to approach it is that it will always be hard for new editors--so we can also focus on making EXISTING editors more productive and effective.</li>
<li> "If you know something that needs to be done but don't have the time, even if it is a 5 minute thing, file a bug report." We should try to encourage that more.</li>
<li> We also need better ways for people to get in touch with existing editors if they have questions. Not having a web chat system hurts a bit probably. (We could iframe freenode's webchat today and have a safe system online!)</li></ul></li></ul></li>
<li> Alex gives us a tantalizing tease: join meeting next week for some good news.</li>
<li> Everyone should feel free to add agenda items for these content meetings.</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="Action_Items_20">Action Items</span></h2>
<ul><li> ACTION: Julee to add to weekly agenda template: "Any new and notable content to promote?" UPDATE: DONE</li>
<li> ACTION: Doug to add folks who responded to email thread as contributing bloggers.</li>
<li> ACTION: Julee and klick_ass to write up WPD blog post about Germany Doc Sprint.  (DONE)</li>
<li> ACTION: Julee to send out Ed Guide outline.  (DONE)</li>
<li> ACTION: Scott to work on usability of Ed Guide.</li>
<li> LAST WEEK ACTION: Julee to update Topic Hierarchy and Architecture pages.  (DONE)</li>
<li> LAST WEEK ACTION: Julee to send out an email discussing how we should "take" and re-assign bugs to even the work out more.  (DONE)</li>
<li> LAST WEEK ACTION: Eliot to do an editorial pass on the proposed top-level pages. UPDATE: No status. now [DONE]</li>
<li> LAST WEEK ACTION: Jswisher to request the next level of detail on the global nav and how the reader accesses the content types as well as the technology areas. UPDATE: Janet sent out the email.</li>
<li> PREVIOUS ACTION: Julee to find out how to add a meeting bot to the Content TF Meeting.  (DONE)</li>
<li> PREVIOUS ACTION: Julee to file a bug about the design of reference pages with a non-standard standardization status.  (DONE)
<ul><li> For needing the categories</li>
<li> For needing the UI updated to reflect the categories</li></ul></li>
<li> PREVIOUS ACTION: Garbee to send out his awesome task organization plan. UPDATE: sending it out today.</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="Agenda_2012-12-13">Agenda 2012-12-13</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> Triage of new content architecture issues
<ul><li> All <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/buglist.cgi?product=webplatform.org&amp;component=content&amp;resolution=---&amp;list_id=2513">content bugs</a> are assigned to either Chris or Garbee. Do we want to re-assign some of them?</li></ul></li>
<li> Top-level navigation and design update from Chris Mills
<ul><li> <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2012Dec/0172.html">Main landing page prototypes completed/subpage structures?/domain leads?</a></li>
<li> <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2012Dec/0235.html">allow people to start their search by technology or page type</a></li>
<li> <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2012Dec/0221.html">Different ways to browse</a></li></ul></li>
<li> Anything blocking you from creating great content?</li></ul>
<p><br />
</p>
<h2><span class="mw-headline" id="Meeting_summary_3">Meeting summary</span></h2>
<h3><span class="mw-headline" id="Discussion_18">Discussion</span></h3>
<ul><li> Note that the <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/buglist.cgi?product=webplatform.org&amp;component=content&amp;resolution=---&amp;list_id=2513">content bugs</a> are assigned to either Chris or Garbee. We wonder how do we spread these out to others? Maybe a larger issue than with just the content bugs?</li>
<li> Discussed top-level pages sent out by Chris. We generally thought Chris's <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2012Dec/0172.html">proposed pages</a> were excellent. Eliot volunteered to do an edit pass on the descriptions. [DONE]</li>
<li> We discussed the <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2012Dec/0235.html">navigation proposals</a> (and <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2012Dec/0221.html">Proposal for updating links on webplatform.org proposal for updating links</a>) that have been in the email list. We discussed the pros and cons of providing the reader with a choice of content type or topic area, via hover links on the global nav. We would appreciate a mock-up. We are not sure how the different proposals would actually pan out. Jswisher took the action to follow up in the email threads and request the next level of detail.</li>
<li> We identified four priorities we're working on to make editing the site easier and hope to have this work completed by the new year:
<ul><li> The global nav/landing pages, discussed above, that Chris Mills is working on</li>
<li> The <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=20160">consolidation of editorial pages</a> that Garbee is working on</li>
<li> Updating the Topic Hierarchy and Architecture pages that Julee is working on</li>
<li> The <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=19390">session bug</a> that shepazu hopes will be resolved this weekend.</li></ul></li>
<li> The Content Task Force will not meet for the next two weeks. We will resume again 1/3/2013.</li></ul>
<h3><span class="mw-headline" id="Action_Items_21">Action Items</span></h3>
<ul><li> Julee to update Topic Hierarchy and Architecture pages.</li>
<li> Julee to send out an email discussing how we should "take" and re-assign bugs to even the work out more.</li>
<li> Eliot to do an editorial pass on the <a rel="nofollow" class="external text" href="http://lists.w3.org/Archives/Public/public-webplatform/2012Dec/0172.html">proposed top-level pages</a>. [DONE]</li>
<li> Jswisher to request the next level of detail on the global nav and how the reader accesses the content types as well as the technology areas.</li>
<li> LAST WEEK ACTION: Julee to find out how to add a meeting bot to the Content TF Meeting.  (DONE)
<ul><li> UPDATE: in progress</li></ul></li>
<li> LAST WEEK ACTION: Julee to file a bug about the design of reference pages with a non-standard standardization status.  (DONE)
<ul><li> UPDATE: needs to be revised: Julee to file a UI bug about the design of reference pages with non-stable status, so that they look distinct.  (DONE)</li>
<li> Filed two bugs:
<ul><li> <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=20386">For needing the categories</a></li>
<li> <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=20387">For needing the UI updated to reflect the categories</a></li></ul></li></ul></li>
<li> LAST WEEK ACTION: Garbee to send out his awesome task organization plan
<ul><li> UPDATE: still working on it</li></ul></li></ul>
<h2><span class="mw-headline" id="Agenda_2012-12-06">Agenda 2012-12-06</span></h2>
<ul><li> Roll call</li>
<li> Review of open action items</li>
<li> Triage of new content architecture issues
<ul><li> Identifying stable vs. proprietary and experimental features</li>
<li> Style guide for example code [<a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=20227%7Cbug">20227</a>]</li>
<li> Topic hierarchy needs updating</li></ul></li>
<li> Anything blocking you from creating great content?</li>
<li> [<a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=20180%7CMain">bug of site UX</a>]
<ul><li> Please review, especially in terms of content discoverability</li>
<li> [<a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=20250%7CBug">on adding a menu</a>]</li>
<li> [<a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=19386%7CBug">for fixing top-level buckets</a>]</li></ul></li>
<li> New templates this week: listing pages</li>
<li> 12/12/12 DocSprint?
<ul><li> Any content-specific focus?</li>
<li> Going? Going to be on IRC? </li></ul></li>
<li> [<a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/buglist.cgi?product=webplatform.org&amp;component=content&amp;resolution=---&amp;list_id=2496%7Ccontent">bugs</a>]: Content bugs in bugzilla need your input and resolution.</li></ul>
<h2><span class="mw-headline" id="Meeting_summary_4">Meeting summary</span></h2>
<h3><span class="mw-headline" id="Topics_discussed">Topics discussed</span></h3>
<ul><li> We discussed the status on the project/program manager for the content tasks. Alex said he realized that the term "project manager" might have caused some confusion and may have implied too big a scope. Really, it's more about someone who just follows through on Action items. We're continuing to discuss this with those who have volunteered for the role.</li>
<li> We discussed categorizing the features as stable, proprietary, experimental, and so on.We do have a page that calls out the different statuses: <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/Property:Standardization_Status">http://docs.webplatform.org/wiki/Property:Standardization_Status</a>. We need to further discuss what are the appropriate categories for WPD. The <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Pillars">http://docs.webplatform.org/wiki/WPD:Pillars</a> page says that we should aim to be useful documentation for the web as it is, so categories such as "proprietary" are important, because we might document something that's useful but has legal restrictions. If there's something TOTALLY proprietary, we had talked about having that in a special vendor section as well </li>
<li> We discussed the example code style bug <a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=20227%7CBug">20227</a>, but decided to table it for a couple of weeks, because Lea's dabbler code highlighting might land next Friday. (Here's what we have so far: <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Manual_Of_Style/Sample_best_practices">http://docs.webplatform.org/wiki/WPD:Manual_Of_Style/Sample_best_practices</a>)</li>
<li> Topic hierarchy page and architecture page is one place where people go to figure out where things go and where they will be. It needs updating. Julee volunteered to do this. We predicted that questions will probably arise from this task.</li>
<li> We want to ask each week: Anything blocking you from creating great content? This week, it's the session bug. Ryan has installed the newest version of mediawiki. There are a few conflicts, he's working to resolve those before deploying.</li>
<li> We called out the user experience bugs for this task force to review, especially to confirm designs are discoverable, accessible, and follows content architecture:
<ul><li> <a rel="nofollow" class="external free" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=20180">https://www.w3.org/Bugs/Public/show_bug.cgi?id=20180</a> (site organization)</li>
<li> <a rel="nofollow" class="external free" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=20250">https://www.w3.org/Bugs/Public/show_bug.cgi?id=20250</a> (global nav)</li>
<li> <a rel="nofollow" class="external free" href="https://www.w3.org/Bugs/Public/show_bug.cgi?id=19386">https://www.w3.org/Bugs/Public/show_bug.cgi?id=19386</a> (links from main)</li></ul></li>
<li> This brought up another topic:</li>
<li> Use Meta bugs on bugzilla are big and fuzzy. Plans, proposals, and scratch pad work should be kept as subpages: <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Plans">http://docs.webplatform.org/wiki/WPD:Plans</a>. Not in Bugzilla, and not in another site, such as GitHub. They keep the substantive discussion/plans in WPD:Plans/FOO, and then as actionable sub-items pop out, we file them as bugs that the meta bug depends on.</li>
<li> Garbee mentioned that one of the things with using Bug genie is we can edit comments.  So we could actually use that as our place to put things like my Beginner's Guide outline as a comment, then just edit that comment when we update things.  Further centralizing some creation there if we 1) Go with Bug Genie and 2) decide to use it that way. So an issue is just opened for it to be created, then the outline is one of the comments.</li>
<li> When new templates appear, such as the listing pages that were sent out for review this week, call it out in terms of content, reviewing it to make sure they make sense from content perspective.</li>
<li> We talked about the coming DocSprint at Google. Several folks are going. Several suggestions regarding promoting, gathering like-skilled folks together via tweeting and other social channels. Also several folks are going to try to get editors' feedback about their experience of the site.</li>
<li> We talked about the template corp and giving access to those who want to edit templates. But not on a one-off basis, more like giving group access.</li></ul>
<h3><span class="mw-headline" id="Decisions">Decisions</span></h3>
<ul><li> Until we have a project management system in place, plans, proposals, and scratch pad work should be kept as subpages: <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Plans">http://docs.webplatform.org/wiki/WPD:Plans</a>. Not in Bugzilla, and not in another site, such as GitHub.</li></ul>
<h3><span class="mw-headline" id="Action_items_22">Action items</span></h3>
<ul><li> Julee to find out how to add a meeting bot to the Content TF Meeting.  (DONE)</li>
<li> Julee to file a bug about the design of reference pages with a non-standard standardization status.  (DONE)</li>
<li> Eliot to update bug 20227 with pointer to the style guide he wrote (DONE)</li>
<li> Garbee to send out his awesome task organization plan</li>
<li> Scott and Peter to explore social media channels about next week's docsprint</li></ul>
<p>Proposed next discussion topics
</p>
<h2><span class="mw-headline" id="Agenda_2012-11-28">Agenda 2012-11-28</span></h2>
<ul><li> Roll call</li>
<li> Triage of new content architecture issues</li>
<li> Review of open action items
<ul><li> The <a href="/wiki/WPD:New_Page" title="WPD:New Page">New_Page</a> page is up to date with example text and links</li>
<li> just like the Getting Started page which has a <a href="/wiki/WPD:Getting_Started#Guides_to_creating_pages" title="WPD:Getting Started">section that anticipates additional guides</a> with a link to</li>
<li> the <a href="/wiki/WPD:Creating_API_pages" title="WPD:Creating API pages">Creating API Pages guide</a>, where all of the above is captured, if not tamed.</li>
<li> Action item for Mike and Julee to try out structure resulted in some issues which we'll continue to discuss today. (See Mike's email to public list 2012-11-15 re: creating api pages.)</li></ul></li>
<li> Handling specialized API <a href="/wiki/WPD:Creating_API_pages" title="WPD:Creating API pages">in light of new guidelines</a>.
<ul><li> How to represent constants and exceptions on separate pages?</li>
<li> Should APIs that add members to existing core interfaces be listed separately?</li>
<li> Where appropriate, note the DOM node used to access each interface object: document, navigator, window, video, audio, etc.</li></ul></li>
<li> <a href="/wiki/WPD:Task_Roadmap" title="WPD:Task Roadmap">Task roadmap</a> includes content track, prioritizing content issues. (See email re: task roadmap for content, infrastructure and styling tasks from Chris Mills &lt;cmills@opera.com&gt;.)</li>
<li> [<a rel="nofollow" class="external text" href="https://www.w3.org/Bugs/Public/buglist.cgi?product=webplatform.org&amp;component=content&amp;resolution=---&amp;list_id=2496%7Ccontent">bugs</a>]: Content bugs in bugzilla need your input and resolution.</li></ul>
<h2><span class="mw-headline" id="Meeting_summary_5">Meeting summary</span></h2>
<h3><span class="mw-headline" id="Topics_discussed_2">Topics discussed</span></h3>
<ul><li> We asked editors to review, update, address content bugs in the bug base: <a rel="nofollow" class="external free" href="https://www.w3.org/Bugs/Public/buglist.cgi?product=webplatform.org&amp;component=content&amp;resolution=---&amp;list_id=2513">https://www.w3.org/Bugs/Public/buglist.cgi?product=webplatform.org&amp;component=content&amp;resolution=---&amp;list_id=2513</a></li>
<li> We pointed out the new task roadmap: <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:Task_Roadmap">http://docs.webplatform.org/wiki/WPD:Task_Roadmap</a>, and related email, and asked for comments. It's a high-level view that's very readable. Editing it (e.g.: adding columns) might be a bit tricky.</li>
<li> We discussed the need for a project management system and a program manager to ensure content tasks are triaged. WPD:Most_Wanted_Tasks isn't working and we need motivational leaders and tools.</li>
<li> We continued discussion on creating API pages, focusing on exceptions to the guidelines (WPD:Creating_API_pages).
<ul><li> What to do for API that add members to an existing interface. For example, CSS Regions includes a new member in the Document interface - keep it with the API or the existing interface? Probably in both. But where does canonical page reside?</li>
<li> What to do with lots of little bits of information, for example SVG attribute values or the HTML type element? For data modeling purposes, it might be best to create separate pages for each and then include them in the main page. What is best for folks importing, managing content? For the end-user?</li></ul></li>
<li> We need to change the meeting time.</li></ul>
<h3><span class="mw-headline" id="Decisions_2">Decisions</span></h3>
<ul><li> We will use bug base for tracking content areas that need to be created, such as DOM ranges.</li>
<li> Until project management for whole project is resolved, we will call out high-level direction on WPD:Task_Roadmap and track specific content issues in bug base.</li>
<li> We will file content bugs on any additional open issues with the API.</li></ul>
<h3><span class="mw-headline" id="Action_items_23">Action items</span></h3>
<ul><li> chrismills to set up a Doodle poll for next meeting times.</li>
<li> garbee to write guidelines on creating content bugs.</li>
<li> (was julee, is now) Garbee to write down (in bug creation guidelines) what issues go where (Bugzilla vs. WPD:Task_Roadmap, WPD:Most_Wanted_Tasks, Special:WantedPages, WPD:Getting_Started, etc.)</li>
<li> Alex to write up a description of the project manager's role.</li>
<li> All: review this summary to ensure accuracy.</li></ul>
<h3><span class="mw-headline" id="Proposed_next_discussion_topics">Proposed next discussion topics</span></h3>
<p>Address any open issues with concepts and tutorials pages.
</p>
<!-- Saved in parser cache with key wpwiki:pcache:idhash:14987-0!*!0!!*!*!*!esi=1 and timestamp 20150731185007 and revision id 45421
 -->
