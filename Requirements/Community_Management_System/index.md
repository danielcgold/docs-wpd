== Description ==
Unearthing requirements for an ideal WPD content and community management system

Also, search within project '''&CCMS'''

== Design choices ==
# Technology choice should be all Javascript. 
# API for content, partial, anything
# Everything end-up in a Git repo

== Backlog ==
Proposed initial backlog:
* As a person, I want to subscribe so I can be known as a user;
* As a user, I want to start contributing by declaring my intention;
* As a user, I'd like to know which pages I should start with;
* As a coordinator, I want to know who said would work ''tonight'';
* As a user, I want to say on which document I am working on;
* As a user, I want to tell when I am done working on a document;
* As a coordinator, I want to give a list of documents that needs to be worked on;
* As a system, I want to make sure a user has access to whatever he has access to;
* As a coordinator, I want to assign tasks to a user;
* As a coordinator, I want to know what a user has been working on recently;
* As a coordinator, I want to know all users who have contributed, but have not contributed recently;
* As a coordinator, I want to know whom I've emailed (or otherwise contacted) and when;

== Functional requirements ==
* Flagging/tagging (users, pages, category)
* Object oriented CMS
** element knows that it needs links, attributes, API, other elements in same category
** [http://www.neo4j.org/ Relationship graph]
 
=== Task allocation system ===
* list of desired task
* easy checkbox to claim task
* file status and time spent
* report on all tasks
* see [http://project.webplatform.org/contributordashboard contributor dashboard]

== Content ==

Content could be organized in small blocks (feature summary, feature code samples, etc) in a way where we can build views depending of the context. Views could be in listing pages, code samples, etc. and be served through an API.