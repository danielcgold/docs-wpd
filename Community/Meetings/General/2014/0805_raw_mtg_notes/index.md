   scribenick: renoirb
   shepazu: Amelia can you update us on the QASprint
   Amelia: yes, as you might have seen the mailing ilst, i've been reorganizing list
   ... there is still close to thousand of articles
   ... beyond that, we discussed about details in the templates and other things to change, but we will work on that later
   Jen: If takes longer and longer; we should be able to keep going and eventually get it all done
   shepazu: opinion
   ... ?
   shepazu: Personally I would there might be value in the idea of "declaring victory" on a set of pages
   ... I heard Eliot and we should hold off until its complete, so I have mixed feelings, maybe we should do nothing until a few more weeks
   Jen: The homepage has those boxes (columns) saying about readiness. I'm not sure if its a good idea anymore because the pages themselves has the flag individually
   ... if that’s the case, we should figure out now how which ones belong to which columns
   (sorry, lost the last 30 seconds)
   Amelia: you are right, at some point we should make sure that the categories are in the right places since we will have a set of real data to help us categorize
   ... to get toward everything there is: DOCUMENTED
   renoir [agrees]
   julee: can you double check If i forgotten something?
   ... make sure we document what we is documented.
   AmeliaBr: Sounds good
   http://docs.webplatform.org/wiki/Special:Log/comments
   renoirb: we should also look at the commenting system that has maybe migrated to issues
   ... e.g. @18:52, 4 July 2014 Caraya (Talk | contribs) + comment (webgl#comment-478 - IE 11 now supports WebGL and it is active in Safari 8 (iOS8 and OSX 10.10))"
   Jen: thanks for pointing that out, I wasnt aware of it.
   ... comments arent going to be issues its conversation
   renoirb: right, but we might have issues hidden there, I wanted to make you aware of it
   julee: we might want to consider assigning "owners" of particular parts
   ... ownership of parts is impressive, i've seen it in the works on MDN. I have been refereed by a community member about an issue on CSS and it was a volunteer who were answering to me
   ... of course we are groing "organically" but in the long run we might like to go toward that
   shepazu: I like julee’s inspiration, but share Amelia’s concern about long term commitment for volunteers
   ... its not as quite robust as it could be
   Jen: The important is to make components available for reuse and visible by the community so people can see and contribute, which is better than the current state.
   Julee: there should be community management plan
   ... have a "community initiative" for next launch
   shepazu [agrees]
   ... I'm working internally to have some W3C team folks to come in
   ... and help us, since they are also actively working on it
   TOPIC: Translation
     http://project.webplatform.org/content/issues/111
     http://project.webplatform.org/content/issues/113
   Jen: I created two issues [113, 111] to document what we discussed last week.
   ... we should continue summarizing the tasks and getting in touch
   ... before going further
 jensimmons:   Here’s the ticket I creted: http://project.webplatform.org/content/issues/111
 jensimmons:   about translation documentiong
 jensimmons:   (I created a ticket about documentation on how people can help with translations, not about whatever ren. is talking about right now)
 renoirb: < pointed out about a possibility to see i18n extensions, maybe there’s improvement compared to what we had when we deployed current version
 TOPIC: Compatibility tables
 shepazu: can you update us renoir
 (renoir updated)
 ... instead of putting in place a technical infrastructure.
 ... we should just have them send an email, or send a bug that says: Hey that page, the data name is wrong. Then somebody else can look it there and change the json file so it gets the correct name and have the result
 renoirb: [agrees]
 ... the question is: How do we surface that. Maybe to add an error message explaining whta to do, e.g. a link to creating an issue in the issue tracker
 ... lets get off list with renoir to see how to change the extension to help the users so we dont rely on templates
 [Renoir stopped scribing, AmeliaBr continues]
 TOPIC: Bugs with Dabblet (code.webplatform.org in IE11)
 shepazu: This is a major concern.  We need to make a new process to always test in all major browsers before deploying things.
 ...currently, renoirb tests what he can, and then sends a note out to the email list asking for people to test and give feedback, but it isn't really structured.
 julee:  We really need to test things properly before we deploy.  This has to happend.
 shepazu:  We understand that, we just need to have a structure, a standard process to follow this.
 renoirb [agrees]
 eliot:  proper testing is a requirement, not a feature request.  Anything that I can do to help that, let me know
 renoirb:  Important point: we all know that testing is primordial.
 shepazu: Well, for starters, any time renoir sends out a note that he has something ready for last testing, you can make sure that one of your team at Microsoft is able to look through it.
 renoirb:  ... we are in the catching up process. Lets work toward improving.
 eliot: Of course.  But we want to do this before things are deployed, not catching bugs later.
 @julee:  My idea was: one table to point members to, so they can do the minimum tests
 shepazu:  exactly.  And if it turns out to be a major problem, maybe we will want to switch to a different system (vs Dabblet), one which has wider support community
 @julee:  That way, Renoirb doesn't have to remember to do all the testing himself.
 @julee:  bye!
 eliot:  For this case, we're looking in to it and it looks like it might be a quick fix.
 renoirb, can you compile the IRC transcript and send the note to the mailing list?