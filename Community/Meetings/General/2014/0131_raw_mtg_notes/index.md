---
title: 0131 raw mtg notes
uri: 'WPD:Community/Meetings/General/2014/0131 raw mtg notes'

---
    julee
    9:02 can anyone scribe?
    renoirb
    9:05 scribenick: renoirb
    9:05 imaginarysteve [~imaginary@174.46.125.167] entered the room.
    renoirb
    9:05 AGENDA: The JS Import
    9:06 Max: A few pages are in the way
    9:06 ... should move them out of the location. mass move them
    9:06 ... some seems to be good enough: libraries and tutorials
    9:06 ... but others could be selected manually
    renoirb
    9:07 Julee: I can do that no problem
    renoirb
    9:07 ... move to Meta namespace so we can use for merge work later down the road
    renoirb
    9:08 Max: I do not want to pressure you Julee... but if you do it in within next 6 hours. I can do that today
    9:08 Julee: yes i can totally do that
    renoirb
    9:09 ... I will move the current 'javascript' with all the children (MW gives the option)... and create a new javascript blank page
    eliezerb
    9:10 \o/
    renoirb
    9:10 Max: The import do not create a 'javascript' landing page
    renoirb
    9:10 Julee: I'll create that top level page no problem
    renoirb
    9:11 ACTION: Max to do the final import tonight
    9:11 ack next
    9:11 AGENDA: Blog posts from Max & Eliezer
    renoirb
    9:11 Julee:  I saw the google docs you started
    renoirb
    9:12 Eliot: We'd like to cover the structure and more whats going on than the technical aspects
    9:13 Max: i can write the blog post
    9:13 ACTION: Max to write blog post draft
    9:13 ack next
    9:13 Eliot: Please make sure the tone is friendly/funny
    9:14 ... we want to cheer up blog post tone
    9:14 AGENDA: Preparing for Web Platform Wednesdays restart with JS content
    renoirb
    9:15 Julee: We are going to focus on EcmaScript v @@
    renoirb
    9:16 ... we are going to work from a spreadsheet instead of MW table
    eliezerb
    9:17 We could create a Open Badge
    renoirb
    9:17 ... to use this to know where to work on and I'll make reports based on that
    renoirb
    9:17 Julee: We had the firestarter and we should have a new badge
    renoirb
    9:17 ACTION: To ask Doug if he wants to create a new badge
    9:18 Eliot: We should make sure people to approve it
    9:18 dobalina [~dobalina@gateway/tor-sasl/dobalina] entered the room.
    renoirb
    9:18 Julee: Anyone can create a badge. We send it to the list and in a General meeting, group can approve it.
    9:19 ptressel left the room (quit: Remote host closed the connection).
    renoirb
    9:19 Julee: 1 Badge to create that badge for the JS project
    9:20 jorgepedret [~jorgepedr@70-36-56-110.dyn.novuscom.net] entered the room.
    renoirb
    9:20 ... If somebody wants to create a badge
    9:20 ... he just have to propose on the mailing list, and the group will approve it
    9:21 AGENDA:  Golden standard
    julee
    9:22 previous agenda items were:
    9:22 rasmusebbesen [~rasmusebb@109.202.139.50] entered the room.
    julee
    9:22 * JS Import
    ** Final import
    ** Blog posts from Max & Eliezer
    * Preparing for Web Platform Wednesdays restart with JS content
    ** Spreadsheet & landing page are done
    ** We need another badge, no?
    9:22 Now: Golden standard
    9:23 shepazu [~shepazu@192.150.22.55] entered the room.
    9:23 mode (+o shepazu) by ChanServ
    renoirb
    9:23 Julee: Is there somebody who wants to make a golden standard
    9:24 rasmusebbesen left the room (quit: Read error: Operation timed out).
    renoirb
    9:25 Eliot: Every page should review and be compared to a list that fits against the standard spec
    renoirb
    9:25 Julee: I will have a spreadsheet all specs and their documents
    renoirb
    9:26 ... On that, we need to have a page to use as an example (hence: Golden standard page)
    9:26 ... that include examples
    9:26 ... links and references
    9:27 ... so we need that ONE VOLUNTEER to make that example page
    9:27 ... and the community to review it
    9:28 ACTION: Somebody to find a volunteer for that Golden page :)
    9:28 shaunbak_ left the room (quit: Remote host closed the connection).
    renoirb
    9:29 Julee: Also we can accept people to volunteer on specific section of a content page
    9:29 shaunbaker [~shaunbake@2001:67c:90:7ff:154f:675:6ac9:a6e9] entered the room.
    renoirb
    9:30 ... I am suggesting that we use the Array page as the candidate to be the page to use
    9:30 renoirb: agrees with the Array page
    9:30 jorgepedret left the room (quit: Quit: Computer has gone to sleep.).
    renoirb
    9:30 AGENDA: Schedule
    renoirb
    9:31 JuleE: there is about 360 pages
    renoirb
    9:31 ... with various levels of information depth
    9:32 ... if we target about 50 pages a week. We are maybe looking at 6 months of work
    9:32 ... lets see how many contributors we have.
    9:32 ... we are going to have a few DocSprints coming in.
    9:32 ... a lot can be done during those
    9:33 shaunbaker left the room (quit: Ping timeout: 245 seconds).
    renoirb
    9:33 Eliot:  Due to the number of DocsSprints, we are looking at a 6 months as a baseline
    julee
    9:34 AGENDA: Site stability
    9:34 renoirb: last time, after the migration, load balancing was needed between server instances
    9:34 … I'm in the process of moving around the VMs
    9:35 … it's a slow process. Not to do during the wee.
    9:35 … I'll do it on the weekends.
    9:35 … A blocker is that 1 isn't being used at all.
    9:35 … We'll use that 4th one for swapping.
    9:35 arnaudb left the room (quit: Remote host closed the connection).
    julee
    9:36 … I'm also fine tuning install, adjust apache servers between servers.
    9:36 julee: how long to get to HA 99%
    9:36 ?
    9:36 renoirb: right now it works well.
    9:37 … there's a lot of work to do.
    9:37 … there's also compatibility table work so I can't work on this all the time.
    9:37 … It's hard to have just one person on this.
    9:37 … There's always something to do.
    9:37 … I want to say next week,
    9:37 … But let's say 1 month.
    9:37 … I have to install tools to make sure.
    9:38 … wish I could have more reassurance.
    9:38 julee: if you install tools, you'll be able to predict better.
    9:38 renoirb : I see in current tools what's happening
    9:38 … But when you see 503s, I need to adjust things.
    9:39 … Errors on servers are always going to be a 503 or whatever.
    9:41 ckwalsh [~ckwalsh@facebook/platform/ckwalsh] entered the room.
    julee
    9:41 julee: predictability first, then HA for contributors
    9:41 renoirb: I know this is important
    9:41 … I am communicating
    9:42 … I have a list I discuss with Doug
    9:42 … We have systems that are giving us information
    9:42 … We just need to make adjustments
    9:42 … We don't have a crystal ball
    9:42 … I need to work on it on the weekend
    9:42 … And then monitor during the week
    9:43 … I like that we make a blog post
    9:43 … and we amplify it
    9:43 morficus [~morficus@108-205-132-58.lightspeed.livnmi.sbcglobal.net] entered the room.
    julee
    9:43 … want to capture the failure for auto communication
    9:44 … and communicating when something happens
    9:44 eliot: I'll help you with a blog post
    9:44 … and we understand the complexity you were handled
    9:44 renoirb: it's not bad, just a big system
    renoirb
    9:45 ... and a lot of loose ends
    julee
    9:45 julee: yes, we appreciate all that renoirb is doing for us
    9:45 renoirb: I have a plan that I communicated with Doug
    9:46 … compatibility tables I'm also working on
    9:46 alrra [~alrra@unaffiliated/alrra] entered the room.
    julee
    9:46 Max: we have an internal test app, bot to load down the servers to test capacities
    9:46 renoirb: that would be nice
    9:46 … I have a system that does a lot of pages
    9:46 … a shell script
    9:47 … but a loadtesting suite, that would be great to get some help to build that.
    9:47 Max: it draws out problems.
    9:47 jorgepedret [~jorgepedr@70-36-56-110.dyn.novuscom.net] entered the room.
    julee
    9:47 renoirb: could you help?
    9:47 Max: sure, it's a longterm project, but yes
    jensimmons
    9:48 for the landing page discussion: http://webplatform.jensimmons.com/design/
    9:48 morficus left the room (quit: Ping timeout: 272 seconds).
    renoirb
    9:49 AGENDA: Compatibility Tables
    julee
    9:49 AGENDA: compatibility tables
    9:50 jorgepedret left the room (quit: Read error: Operation timed out).
    renoirb
    9:50 Pat
    9:50 Pat tressel
    9:50 eliot [836bc090@gateway/web/freenode/ip.131.107.192.144] entered the room.
    julee
    9:50 renoirb: I got in touch with Pat Tressel
    9:50 we are free to work on the compat tables
    9:51 … there had been some discussions about how to represent it
    9:51 ptressel [~chatzilla@174-31-227-126.tukw.qwest.net] entered the room.
    julee
    9:51 … all we want is to import MDN & caniuse for now
    9:51 … eventually, data will come from Testthewebforward
    9:51 … Right now we have the code from Pat to build the HTML tables
    9:52 … We're about to start this taskforce
    9:52 … to use TestTWF
    9:52 … Need to not cut off data that we have from MDN & caniuse
    9:53 … ^ historical data
    9:53 … Testtwf will be additive
    9:53 … browser sniffing as well
    9:53 There are a lot of components
    ptressel
    9:53 (Little correction: The code is from frozenice, rather than Pat.)
    julee
    9:53 … Part of Testtwf project
    eliot
    9:54 Just  a point of clarity: I believe the goal is to uset he W3C test suite (which TestTWF donates tests to)
    julee
    9:54 Julee: can we get a plan?
    eliot
    9:55 q+
    julee
    9:56 Julee: would like to have more visibility on this plan
    9:56 Are we triangulating data
    9:56 What taskforce?
    9:57 What if Testtwf doesn't have test?
    9:57 Are we no longer going to take the contributed data from others and triangulate the data?
    9:57 renoirb: we'll do browser sniffing and push the results
    9:58 Julee: I gues there's already a taskforce & designs, I look forward toseeing some of this.
    9:58 Eliot: Testtwf : tests are donated
    9:59 … the goal is to use this test suite to validate
    9:59 … If no test, spec can't get to Recommendation phase without tests for each normative statement
    9:59 … 6 figures for HTML5 of tests
    9:59 …  10K tests are being donated!
    10:00 … All specs need these test
    10:00 … Ultimately, that's what we're going for
    10:00 alrra left the room (quit: Quit: Leaving).
    julee
    10:00 … And then if we have sites that don't use normative tests, do we use that data?
    10:01 … More like building a test harness than juggling folks who are creating these tests
    10:01 jen: hope we still have a human element, here
    10:01 eliot: Yes
    10:01 … And what if spec doesn't have tests
    10:02 jen: really is a resource : can I really use this right now
    10:02 … test harness is great, but when data is aggregated and triangulated, it gives a human reality check
    10:03 eliot: yes, but for the purpose of the compatibility table : it is about the data
    10:03 jen: that's not how folks use caniuse
    10:03 eliot: We're saying teh same thing
    10:03 jen: but maybe we have different definitions of whether something works
    10:03 … real word level of specs not working out
    10:05 julee: The taskforce should be announced
    10:05 … and plan should be published so folks can comment on it
    renoirb
    10:06 scribenick: renoirb
    jensimmons
    10:06 http://webplatform.jensimmons.com/design/
    renoirb
    10:06 Jen: If you go to ^
    10:06 ... you see a prototype in progress
    10:06 ... should get the idea of the model
    10:06 ... could get the idea of the content hierarchy
    10:07 ... do not look at the lower section
    10:08 jorgepedret [~jorgepedr@64-46-23-103.dyn.novuscom.net] entered the room.
    10:08 arnaudb [~arnaudb@72-18-233-188.static-ip.telepacific.net] entered the room.
    renoirb
    10:08 ... for the first page, doesn't matter if we have to update some of the content in the html directly
    10:09 ... make sure that content such as next doc sprints
    10:09 jorgepedret left the room (quit: Read error: No route to host).
    10:10 jorgepedret [~jorgepedr@64-46-23-103.dyn.novuscom.net] entered the room.
    renoirb
    10:10 ... opinions
    10:11 Eliott: I really like the direction you are going with this
    renoirb
    10:11 Julee: this is more what we need
    10:11 jonatasnona left the room (quit: Ping timeout: 240 seconds).
    renoirb
    10:12 Jen: I just wanted to give direction, we should definitely agree with the content
    renoirb
    10:14 renoirb: seconds about Eliot and Julee
    renoirb
    10:14 adjourned
