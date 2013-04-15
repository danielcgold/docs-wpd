=DOM API documentation=

This is the project page for the DOM API documentation on WPD.

==Purpose==

The purpose of this documentation is to describe the Document Object Model for developers of applications that work with DOM artifacts. It is not an architectural study of the DOM, nor is it intended to support the development of the DOM itself.

==Scope==

This documentation will cover the programatic artifacts that provide an interface to the DOM, the APIs. This document does not cover the HTML elements or CSS artifacts that otherwise are considered part of the DOM. Nor does this project deal with the SVG or MathML content in WPD.

==Tasks==

The two primary tasks of this project are as follows:
* Reorganize the DOM API documentation in a coherent structure that supports short, predictable URLs.
* Fill in the pages with information currently missing.

==Reorganization==
First, we have to reorganize our current content.

===Organization problems===
Most of the problems with the way the content is currently organized boil down to the use of "interstials" - either as unnecessary namespace delineations or artificial subtree designations.

Consider the current state of the [[dom|DOM]] pages. Some follow the very plain, short, and predictable delineation that we consider optimum:
* dom/<object>/<member>
Where <member> may be a property or method. For example,  [[dom/Element/error]].

Some pages are designated as subtrees of the dom/apis. These are:
* [[dom/apis/audio-video]]
* [[dom/traversal]]
These subtree designations appear to be completely artificial, unlike the use of such designations in the [[WPD:Creating_API_pages|API Project]], where API_Listing pages described the common name of the API. The member pages of these dom "subtrees" invariably refer to their parent objects, though these are not shown in the URL.

Other pages are using "interstitials" to describe the namespace type, such as:
* dom/apis/<object>/<member>
For example, [[dom/apis/document/getElementById]]. Note the object name, "document" is not capitalized, which violates our rules of capitalization. 

Interstitials are used to delineate objects and members:
* dom/objects/<object> 
* dom/events/<event>
* dom/methods/<method>
* dom/properties/<property>
For example [[dom/events/abort]] or [[dom/methods/moveTo]]. For members, these lack any description of the objects that encapsulate them in the URL, though usually the reference to the parent object is maintained in the content.

Also, within named subtrees of the dom/apis, interstitials are used to distinguish methods and properties as well as events. For example, [[dom/apis/audio-video/properties/type]].

Some pages have no interstitials at all.
* dom/<member>

For example, [[dom/gotpointercapture]].

Inheritance is not described in the URLs of the pages. Most pages follow this organization:
* dom/<object>
For example, [[dom/HTMLTrackElement]] ''not'' [[dom/EventTarget/Node/Element/HTMLElement/HTMLTrackElement]].

===Organization solution===

Proposed is the abolition of all "interstitials" except for the "event" interstitial, and the assignment of all members to their encapsulating objects in the URLs. Even the "apis" interstitial is unnecessary (see below). To that, we would have the following first-tier designations.
* '''dom''' - a listing page with all DOM objects and their summaries.
* '''dom/events''' - a listing page with all DOM events

Events are usually targeted to DOM Elements, and the event target is not information that need be displayed in the URL. However, the designation of events as separate from other DOM artifacts is useful as information in the URL.

Inheritance, however, should not be described in the URL. Rather, all DOM objects, regardless of their "level" in the DOM, should reside on one level of the WPD URL structure. This provides for short URLs. So, we would have the following:
* dom/HTMLTrackElement (''not'' dom/EventTarget/Node/Element/HTMLElement/HTMLTrackElement)
* dom/Navigator
* dom/Window
* dom/Node
* dom/Document
* dom/Element
* dom/HTMLElement
* dom/HTMLMenuElement
etc.

Going further into the namespace, all members would be organized under their parent objects. To wit:
* current: [[dom/apis/document/getElementById]] proposed: [[dom/Document/getElementById]]
* current: [[dom/traversal/methods/RangeException]] proposed: [[dom/Element/RangeException]]

This follows the methodology in the [[WPD:Creating_API_pages|API Project]], except that API_Listing pages are not required to describe interstitials (other than the "dom" and "events" listing pages), because there is no danger of namespace conflicts that would require the use of such interstitials.

An "apis" interstitial is unnecessary. The DOM itself includes CSS, CSSOM, HTML Elements, SVG, etc., and we have already broken out the content into these top-level buckets. We don't have "dom/css/cssom" or "dom/svg." We are designating this bucket as the "dom" to mean the objects and interfaces used to program against the DOM. That these are understood to be the APIs, using "apis" as an interstitial (as in "dom/apis") is redundant. We have only the "events" subtree of the DOM as an interstitial, as it is an area of related usage.