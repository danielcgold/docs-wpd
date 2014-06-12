=Readiness Markers & Editorial Notes=

Readiness markers display information about the quality of an article at a glance.  They are visible to anyone arriving at the site, so that it is clear when work is not complete and caution should be used.  The readiness states are also available to be searched, so that site editors can keep track of work to be done.

Editorial notes are not displayed to people who are coming to WebPlatform Docs for information.  They are only shown in the editing forms, and provide an open-ended way for contributors to indicate what work still needs to be done.  In particular, they should explain what needs to be done before the page can be marked "ready to use".


==Readiness States==
The official definitions for the readiness options are given on their [[Property:State| property page]].  The following explanations describe the purpose of the different states more generally:

===Ready to Use===
A document should be marked Ready to Use if a developer who is looking for reference material on this topic can randomly land on this page and get complete, accurate information. The information on a Ready to Use page is not outdated, and it's not incomplete in a way that would make the information confusing. Much of the documentation on webplatform.org will need to be continuously be revised and updated as standards and techniques change, so Ready to Use pages don't have to always be 100% perfect. They may need minor errors or quick updates.  Hopefully those kinds of edits are simply done as soon as the need for an edit is discovered. In that case, switching the readiness status of the page in a more complex workflow process isn't needed.

===Almost Ready===
A document should be marked Almost Ready if it's 80% ready, but still needs something that's clearly missing or incomplete.  Almost Ready might be used when the descriptions are good, but there are no examples. Or when the editing that humans can do is complete, but there's still something else that needs to be coded in the system to make the pages ready — such as connecting the compatibility tables. This could be used as a way to mark a group of pages for review if an initiative needs such a tool, as a kind of Q/A stage. Or this status might not be used at all; pages can go straight from In Progress to Ready to Use if the circumstances warrant it.

This state was called Almost Done / Almost Complete in earlier discussions of the readiness states.

===In Progress===
A document should be marked In Progress if work on it has officially begun, but it's not close to being ready yet. This marker will tell developers who may stumble across the page — hey, don't trust this documentation yet: It's not a reliable source of information, it's a page that's being heavily rewritten. Any page that's more than 10%, but less than 80% done should be marked In Progress. It doesn't matter whether there is active work being done on it currently or not. 

===Needs Work===
A document should be marked Needs Work when it's just an idea. This can be used when someone has created a page, with a URL and a title, maybe a "stub" summary, but not much else. It should also be used when content is imported from an outside source, but has not been looked at by WPD contributors or restructured for our system yet.

This state was called Coming Later in earlier discussions of the readiness states.

===Out of Date===
A document should only be marked Out of Date if it was previously marked "Ready to Use" or "Almost Done", but is no longer accurate due to changes in the standards or implementations discussed.  Whenever possible, a document should be edited to update it instead of marking it out-of-date.

===Unreviewed=== 
A document is unreviewed if it has not had a state value assigned.  This value should not be set manually.

==Statistics==

Current numbers of articles with each status:
*Ready to Use: ([{{fullurl:Special:SearchByProperty|property=State&value={{urlencode:Ready to Use}}}}  {{#ask: [[State::Ready to Use]] | format=count}} articles])
*Almost Ready: ([{{fullurl:Special:SearchByProperty|property=State&value={{urlencode:Almost Ready}}}}  {{#ask: [[State::Almost Ready]] | format=count}} articles])
*In Progress: ([{{fullurl:Special:SearchByProperty|property=State&value={{urlencode:In Progress}}}}  {{#ask: [[State::In Progress]] | format=count}} articles])
*Needs Work: ([{{fullurl:Special:SearchByProperty|property=State&value={{urlencode:Needs Work}}}}  {{#ask: [[State::Needs Work]] | format=count}} articles])
*Out of Date: ([{{fullurl:Special:SearchByProperty|property=State&value={{urlencode:Out of Date}}}}  {{#ask: [[State::Out of Date]] | format=count}} articles])
*Unreviewed: ([{{fullurl:Special:SearchByProperty|property=State&value={{urlencode:Unreviewed}}}}  {{#ask: [[State::Unreviewed]] | format=count}} articles])
*Other values: ([{{fullurl:Special:SearchByProperty|property={{urlencode:Has improper value for}}State&value=State}}  {{#ask: [[Has improper value for::State]] | format=count}} articles])

==Implementation==

The readiness marker system is now live on the main wiki.  CSS styling still to come.  The implementation depends on the following templates and Semantic MediaWiki properties:

* [[Property:State]]<br/>
The State property defines the readiness state property, and contains definitions of each value (slightly shorter versions of the ones from Jen's email) and links to search pages for each value.  For now, this is the page you get to when you click on the readiness-related link in the form or main article page.    In the future, that may be changed to link to this page.
* [[Property:State_Details]]<br/>
The State Details property will contain any editorial notes related to the page and the reason it was given a certain state.  Nothing prints on the final "View" mode of the article, but by saving the information as a property they can be accessed by search functions (the above link will have a list of all articles with a value set).  Although the property is new, it reuses the "Editorial Notes" form field from the old flags template, which means that any custom editorial notes should be preserved (although it's a little messy, because most of them used their own templates which inject html code).
* [[Template:Flags_Form_Section]]<br/>
The old flags form section template has been reused, so that all pages that previously allowed you to set flags now allow you to set a readiness state.  The revised template has three elements: readiness state, state details/editorial notes, and checked out.  Edit any reference page to see what it looks like in action.
*  [[Template:Flags]]<br/>
Likewise, the old Flags template has been used to print the readiness markers.  Any pages which previously had the option to show flags under the title will instead show the readiness statement (if a value has been set).
* [[Property:Content_quality_flag]]<br/>
The flags property is still used for the automatically-set flags Needs Summary, Examples Needed, and Compatibility Incomplete.  The property page needs to be updated, as does [[WPD:Flags]] and its sub-pages.

==Design==

The state value is printed to the page in the following format by the Flags template:

<syntaxhighlight>
<div class="note readiness-state Almost_Ready"> 
<p>This article is <a href="/wiki/Property:State" title="Property:State">Almost Ready.</a>
</p>
</div>
</syntaxhighlight>

The "note" class is responsible for the current yellow-box display.  The "readiness-state" and state-specific class will be used for the final CSS.  The state-specific classes are created from the property values by replacing spaces with "_", so they are: "Ready_to_Use", "Almost_Ready", "In_Progress", "Needs_Work", "Out_of_Date".  (The "Unreviewed" value currently never results in a div being added to the page.)

You can find the latest discussion about (and examples of) the proposed design for the markers on the [http://lists.w3.org/Archives/Public/public-webplatform/ webplatform email list].