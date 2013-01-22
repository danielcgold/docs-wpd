{{Page_Title|Suggested design enhancements for CSS properties}}
{{Flags}}
{{Summary_Section|This page [http://letmespellitoutforyou.com/x/webplatform/font_size.html] is a suggested mockup of how a CSS property page should look.
Compared to the [[css/properties/font-size|original page]], there are
several enhancements that would need to be implemented, and here is a
list of the most significant.
}}
{{Basic Page}}
* Page title & summary are on the same line in this example; formatted as left/right justification with negative margin for overlay; this is fragile for cases where text in either runs too long.

* Removed hard-coded "W3C Recommendation" text. If necessary, use a graphic to represent options or otherwise push it out of the main text flow.

* "Specifies the size of text" is currently called a "summary", hopefully a simple sentence reflected in CSS property listings.  The "This property sets the..." text offers more fleshed-out expository context not intended for listings. New field needed in template. What to call it?

* Removed the implicit "Summary" & "Overview table" headings.

* Under "Values", each &lt;dt&gt;/&lt;dd&gt; pair generate incorrectly in its own &lt;dl&gt;, which also produces unnecessary rules. Regardless, Suggest removing the rule formatting altogether as too busy.

* Heavily reformatted property value overview table. Suggest shading all rows white here.

* Each cell title ("Computed value"/"Initial value") should link to a concept page.

* Inherited/Animatable use check/X icons rather than Yes/No text.

* Current template only allows one media type, but property may well apply to more.

* Added an extra "Shorthand" field to overview table. Suggest a field in e.g. template for font-size to specify "font". Then font-size page would display "Shorthand: font" and font page would display "Shorthand for: font-family, font-size, font-weight" ... etc. for all properties that share the same shorthand.

* If property is marked as "inherited", should a syntax line & value description be automatically generated, or is it implicit, and is link to the "inherited" concept sufficient? Authors should not have to redundantly hard-code the "inherit" value at any rate.

* Fixed keyword values are bold, while variables are italic. The template provides no way to make that important distinction.

* Default text for &lt;dd&gt; text in "Values" section should not be italic.

* Heavily reformatted & merged the compatibility table.

* Separated sub-issues in compatibility table (e.g. "vw/vh/vmin viewport units") with col-spanned table headings.

* Under compatibility notes, added less-than/greater-than/equals for explicit relation to version numbers.

* Removed redundant "See Also" head; used "Related Articles" instead. 

* Pushed Specification info into "Related Articles" area

* Reformatted most related-article links as 3-column to save space. (Can CSS formatting kick in after # of list items exceeds a threshold?)

* Directly embedded a sample page as an &lt;iframe&gt;. This is only a suggested UI. Hopefully dabblet sample pages can be presented this way, directly available on the page next to doc that describes it.

* Suggest adding explicit "example" template options for embedded samples, and for images showing the result of CSS formatting.

* Unclear what "Percentages" template option is intended for "Top-Level Summary", but it is not reflected in the resulting overview table.
{{Notes_Section}}
{{Topics}}
{{External_Attribution
|Is_CC-BY-SA=No
|MDN_link=
|MSDN_link=
|HTML5Rocks_link=
}}