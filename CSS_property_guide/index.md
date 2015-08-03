---
title: WPD:CSS property guide
---
<h1><span class="mw-headline" id="CSS_property_editing_guide">CSS property editing guide</span></h1>
<h2><span class="mw-headline" id="Summary">Summary</span></h2>
<p>Help us update, review, add samples, and add quality to the CSS properties! This article is a guide to implementing a CSS property reference page.
</p>
<h3><span class="mw-headline" id="Before_you_begin">Before you begin</span></h3>
<p>Before you begin, you already should have:
</p>
<ul><li> taken the steps to register for this site, communicate with the team, and work with the wiki. (Select <a href="/wiki/WPD:Editors_Guide" title="WPD:Editors Guide" class="mw-redirect">"Editing"</a> from any page on the site.)</li>
<li> ran through at least one basic contribution. (See how to <a href="/wiki/WPD:Getting_Started" title="WPD:Getting Started">start contributing content</a>, and cycle through one basic task, such as fixing a link or adding a summary to a page.)</li></ul>
<h3><span class="mw-headline" id="High-level_steps">High-level steps</span></h3>
<p>Below, Chris Mills runs through updating a property. But basically, you:
</p>
<ul><li> pick a property (preferably one that's priority-0 through priority-2) from <a href="/wiki/Meta:web_platform_wednesday" title="Meta:web platform wednesday">the weekly list</a> and have a coordinator add your name in the owner/reviewer column</li>
<li> read the CSS property page through</li>
<li> compare it to its spec(s)</li>
<li> compare the content to other reputable sites, such as Mozilla Developer Network</li>
<li> play around with the elements documented – you can use our playground <a rel="nofollow" class="external free" href="http://code.webplatform.org">http://code.webplatform.org</a>.</li>
<li> update the page based on your findings</li>
<li> remove any flags you think are no longer necessary</li>
<li> ask a coordinator to update the <a href="/wiki/Meta:web_platform_wednesday" title="Meta:web platform wednesday">the weekly list</a> with your status</li>
<li> send us a message @webplatform to let us know you've done a page and if you'd like a review</li></ul>
<h2><span class="mw-headline" id="Ignore_the_master_CSS_properties_spreadsheet">Ignore the master CSS properties spreadsheet</span></h2>
<p>We have compiled a rather large and hopefully exhaustive list of all existing CSS properties — this can be found at
<a href="/wiki/Meta:web_platform_wednesday/master_list" title="Meta:web platform wednesday/master list">the master list</a>  - but you can ignore this.
</p><p>We have assigned each property a priority level, starting from Priority-0 and going down to Priority-4, where P0 is the highest priority for vital, commonly-used properties that every browser supports. P4, then, is considered the lowest level is for properties, because they're rarely-used, proprietary, have limited cross-browser support, or all of the above. We would like to start on the highest priority ones and work out way down.
</p>
<h2><span class="mw-headline" id="Choosing_a_property_to_work_on">Choosing a property to work on</span></h2>
<p>So the first step is to have a look at which properties you would like to work on. I would suggest grabbing a group of related properties that would work well as unit to work on. So for example, I grabbed
</p>
<ul><li> background</li>
<li> background-attachment</li>
<li> background-color</li>
<li> background-image</li>
<li> background-position</li>
<li> background-repeat</li>
<li> background-size</li>
<li> background-clip</li>
<li> background-origin</li></ul>
<h2><span class="mw-headline" id="Assigning_you_to_work_on_your_chosen_properties">Assigning you to work on your chosen properties</span></h2>
<p>Once you have grabbed some properties to work on, let us know, so we can track who is working on what:  Have a coordinator add your name into 
<a href="/wiki/Meta:web_platform_wednesday" title="Meta:web platform wednesday">the weekly list</a>
Then work through each property until you have completed your set. In this example I will do background-image — see my finished example at <a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/css/properties/background-image">http://docs.webplatform.org/wiki/css/properties/background-image</a>
</p>
<h2><span class="mw-headline" id="Creating_your_page.2C_in_the_right_place">Creating your page, in the right place</span></h2>
<p>First, look for the prior existence of a page about this property on the WPD wiki. The general URL scheme is
</p><p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/css/properties/property-name">http://docs.webplatform.org/wiki/css/properties/property-name</a>
</p><p>So this page should be placed at 
</p><p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/css/properties/background-image">http://docs.webplatform.org/wiki/css/properties/background-image</a>
</p><p>If it already exists, great! Go on to the next step.
</p><p>If not, then it is worth checking whether it exists at the wrong location. First try entering your property name in the WPD search box and see if a specific page turns up. The URL might be wrong — it might have "properties" swapped out for "Properties", or "Background-Image" swapped out for "background-image", or a forward slash on the end of the URL. These all make it a different URL, as Media Wiki has a number of quirks, including case-sensitive URLs.
</p><p>If it already exists in the wrong place, we need to move it into the right place, using the "Move" tool, found in the tools menu when you are logged in. You need to enter a new slug for it to sit at. If there is something already at the new location, it will warn you and ask if you want to delete it. Please don't! We don't want to risk losing valuable content, so make sure you move the existing content somewhere else before moving your chosen content there. A good way to deal with it is to just move the old page to a location of OLD:[slug], for example OLD:background-image.
</p><p>If the page does not exist at all, you need to create a new page, using the New Page creator tool at 
</p><p><a rel="nofollow" class="external free" href="http://docs.webplatform.org/wiki/WPD:New_Page">http://docs.webplatform.org/wiki/WPD:New_Page</a>
</p><p>You can access this by navigating to the URL where you want the page created and clicking on the new page link.
</p><p>You need to use the "CSS Property" section to create a new page for your CSS property. change "css/properties/foo" to "css/properties/property-name" (in my case it would be "css/properties/background-image") and press the "Create CSS property page button"
</p><p>If you are adapting/modifying an existing page, and it has the wrong template assigned to it (you'll know because the edit form won't contain the correct fields) or no template at all (you'll get no edit form when pressing "Edit", just a single textarea containing course code), then the only way to move it to the correct form type is to edit the page source to give it the right form information to use. This often isn't that simple, so either talk to a Webplatform steward for help, or just create a new page and copy the existing information across to it.
</p>
<h2><span class="mw-headline" id="Entering_data_on_the_page">Entering data on the page</span></h2>
<p>Now you are ready to start gathering the data to enter into your page. I'd advise that you gather the data and record it offline first, just in case something stupid happens and you lose your edits. I'm not saying it <i>will</i> happen, but you never know with Wikis! So copy the following headings, put them into your text editor, then read below on how to fill them in.
</p>
<ul><li> Custom page title</li>
<li> Article summary</li>
<li> Data table</li></ul>
<pre>Initial value:
Computed value:
Inherited:
Applies to:
CSS Object Model property:
Media:
Animatable:
Shorthand: (this currently doesn't exist in the CSS property form template but will be added soon. Note the related shorthand property, if one exists, in the notes section for now)</pre>
<ul><li> Syntax</li>
<li> Examples</li>
<li> Usage</li>
<li> Related specifications</li>
<li> Related articles</li>
<li> Compatibility table (You can ignore these for now. We're working on brining in the data manually.)</li>
<li> Compatibility notes (Only add something if you think it's unique and isn't represented on sites like caniuse.com or developer.mozilla.org)</li></ul>
<p>After collecting all the information, you'll then need to go through the different form fields in the edit page and fill each one in.
</p>
<h3><span class="mw-headline" id="Researching_information">Researching information</span></h3>
<p>You should research the information for your article and how to verify its correct, using trustworthy sites like MDN, caniuse, quirksmode and relevant CSS specs. Review existing documentation from other sources and then read the relevant specs. If the sources all agree then you can accept the information as correct, but if they disagree you should do original research or ask for help from more knowledgeable members.
</p><p>When you have finished writing a page, you should get someone else to review it to verify its quality.
</p>
<h3><span class="mw-headline" id="Putting_information_that_applies_to_multiple_properties_in_separate_pages">Putting information that applies to multiple properties in separate pages</span></h3>
<p>NOTE: One important thing you should consider when entering information into your property pages is whether any of that information also applies to other CSS properties. If it does, then you should consider putting that information into a separate page, whether it is a concept, function or whatever. This way, you can save others a lot of time and repetition.
</p><p>So, in the case of my example, url() and *-gradient() functions are viable targets within the "css/functions" tree. I have created a page to cover url() at <a href="/wiki/css/functions/url()" title="css/functions/url()">CSS images: url()</a>, and linear and radial gradients are currently intended to be covered at <a href="/wiki/tutorials/creating_gradients_in_css" title="tutorials/creating gradients in css">Creating gradients in CSS</a>.
</p><p>If you were describing background colors, rather than detail how RGBA/HSLA values work, you could instead point to pages within the "css/units" (whihc doesn't exist yet). If you find yourself using any other common jargon that's hard to classify &amp; that readers might not be familiar with, create a link within the top-level "concepts" tree, e.g., "viewport," "vendor prefixes," or "standards
mode." Readers may also benefit from links to tutorials on the subject available as "CSS learning material." (Other areas such as HTML, JavaScript, and SVG have their own learning material areas.)
</p>
<h3><span class="mw-headline" id="Summary_information">Summary information</span></h3>
<p>First of all, let's start with the summary information near the top of the page.
</p>
<h4><span class="mw-headline" id="Custom_page_title">Custom page title</span></h4>
<p>Enter the property name, for example background-image
</p>
<h4><span class="mw-headline" id="Top_level_summary">Top level summary</span></h4>
<p>Enter a very brief description of function, for example
</p><p>"The background-image property allows you to apply one or more background images to an element. These can be url() paths to image files, or CSS3 linear or radial gradients. For more information, consult <a href="/wiki/tutorials/using_css_background_images" title="tutorials/using css background images">Using CSS background images</a> and <a href="/wiki/tutorials/creating_gradients_in_css" title="tutorials/creating gradients in css">Creating gradients in CSS</a>."
</p>
<h4><span class="mw-headline" id="The_data_table">The data table</span></h4>
<p>This refers to the small fields below the Summary. Fill these data items in as exactly as you can.
</p>
<ul><li> Initial value: none</li>
<li> Computed value: As specified, but with URIs made absolute</li>
<li> Inherited: no</li>
<li> Applies to: all elements</li>
<li> CSS Object Model property: backgroundImage</li>
<li> Media: visual for now (you can't currently specify more than one)</li>
<li> Animatable: yes</li>
<li> Shorthand: background</li>
<li> Percentages (ignore this)</li></ul>
<p>NOTE: computed values and initial values can often be hard to find by searching on your favorite search engine. A better way to find them out is often to create a very quick test (or even just go to an already-existing web page) and play with different values of said property, and see what the computed values are reported as (most browser dev tools, e.g. Opera Dragonfly, Chrome Dev Tools, report computed values.) Sometimes the computed values are not quite as simple as you'd think. For example with the color property, the computed value is always the hexadecimal equivalent, except in the case of translucent colours, where it is always the RGBa equivalent.
</p><p>Note: To check whether you property is animatable or not, write a simple test, or check out a list such as <a rel="nofollow" class="external text" href="http://oli.jp/2010/css-animatable-properties/">CSS animatable properties</a> by Oli Studholme. 
</p>
<h3><span class="mw-headline" id="Syntax_and_values">Syntax and values</span></h3>
<p>Now on to the syntax and value explanations.
</p><p>You should provide a different syntax value all notable different value types, along with a nice detailed explanation, in the <b>Values</b> form fields. These  values are then used to auto-populate the <b>Syntax</b> and <b>Values</b> sections of the page.
</p><p>Here, all the possible value types indicated in the syntax section should be expanded upon and explained clearly
</p><p>for example
</p>
<ul><li> url(path/to/image.png)
<ul><li>	This value contains a path to an image that you want to apply to the element in question as a background image, using the CSS images syntax, as described at <a href="/wiki/css/functions/url()" title="css/functions/url()">CSS images: url()</a>.</li></ul></li>
<li> linear-gradient(to bottom, #f00, #aaa)
<ul><li> 	Programmatically creates a gradient that travels from one side of the element to the other. For more on the syntax, read <a href="/wiki/tutorials/creating_gradients_in_css" title="tutorials/creating gradients in css">Creating gradients in CSS</a></li></ul></li>
<li> radial-gradient(50% 50%, circle, #f00, #aaa)
<ul><li>	Programmatically creates a gradient that radiates outwards from a specified point on the element's background. For more on the syntax, read <a href="/wiki/tutorials/creating_gradients_in_css" title="tutorials/creating gradients in css">Creating gradients in CSS</a>.</li></ul></li>
<li> url(path/to/image.png), url(path/to/image2.png), url(path/to/image3.png)	
<ul><li> 	You can apply multiple background images to a single element (image files, gradients, or a mixture) by including all the image references in the property value, with each one separated by a comma. Images referenced earlier in the property value appear in front of images referenced later.</li></ul></li></ul>
<h3><span class="mw-headline" id="Examples">Examples</span></h3>
<p>For the examples section, you should provide one or two brief examples that succinctly show how to do a real world implementation of the property being shown. You should show your HTML and CSS, and anything else relevant, in separate sections, as provided by the edit page.
</p><p>For example:
</p><p>HTML
</p>
<pre>&lt;!DOCTYPE HTML&gt;
&lt;html lang=&quot;en-US&quot;&gt;
&lt;head&gt;
	&lt;meta charset=&quot;UTF-8&quot;&gt;
	&lt;title&gt;Background-image example&lt;/title&gt;
	&lt;link href=&quot;background-image.css&quot; type=&quot;text/css&quot; rel=&quot;stylesheet&quot;&gt;
&lt;/head&gt;
&lt;body&gt;

&lt;div class=&quot;one&quot;&gt;One&lt;/div&gt;
&lt;div class=&quot;two&quot;&gt;Two&lt;/div&gt;
&lt;div class=&quot;three&quot;&gt;Three&lt;/div&gt;

&lt;/body&gt;
&lt;/html&gt;</pre>
<p>CSS
</p>
<pre>.one {
  background-image: url(images/icon.png);
  /* here we are applying a single background image to our first block level container element */
  /* (could be anything, but it is a &lt;div&gt;in the live example. */
}

.two {
  background-image: -webkit-linear-gradient(top,#aaa,#eee);
  background-image: -moz-linear-gradient(top,#aaa,#eee);
  background-image: -ms-linear-gradient(top,#aaa,#eee);
  background-image: -o-linear-gradient(top,#aaa,#eee);
  background-image: linear-gradient(to bottom,#aaa,#eee);
  /* Here we are applying a linear gradient to our second block level container. */
  /* We have included a line with each different vendor prefix type, so that all supporting */
  /* browsers will have something they can apply. This includes a prefixless version of the */
  /* property, which uses the latest version of the syntax for the spec. As browsers update their  */
  /* implementations and drop their prefixes, tyhey can start to use this syntax instead, meaning */
  /* that the code will still work. */  
}

.three {
  background-image: url(images/icon.png), -webkit-linear-gradient(top,#aaa,#eee);
  background-image: url(images/icon.png), -moz-linear-gradient(top,#aaa,#eee);
  background-image: url(images/icon.png), -ms-linear-gradient(top,#aaa,#eee);
  background-image: url(images/icon.png), -o-linear-gradient(top,#aaa,#eee);
  background-image: url(images/icon.png), linear-gradient(to bottom,#aaa,#eee);
  /* In this case we are applying both the background image and the gradient to our third block level container. */
}</pre>
<h4><span class="mw-headline" id="Live_examples">Live examples</span></h4>
<p>At a slightly later date, we are intending to integrate <a rel="nofollow" class="external text" href="http://dabblet.com/">Dabblet</a> with our site, so we will be able to have live examples running inside our references and tutorials. Until the live example viewer is properly implemented, we would suggest just showing the source code in the page for now, as instructed above. In my finished example page, I have hosted a live example at Github; feel free to host a live version at Github or another place if you feel like it.
</p><p><br />
</p>
<h3><span class="mw-headline" id="Usage_.28optional.29">Usage (optional)</span></h3>
<p>The Usage section should contain notes that impart useful, practical knowledge about using the property in the real world. What do you really need to know when trying to use this property in production?
</p><p>For example
</p><p>"Background images in general have good support across browsers; there are a few things to take note of, however:
</p>
<ul><li> Older browsers do not support multiple background images, SVG as background images or CSS gradients, so be careful when using these options to make sure that a fallback is provided that will make content readable on older browsers, such as a simple solid colour.</li>
<li> When using multiple background images, the image at the start of the comma delimited list appears on top of ones later on. This might seem contrary to how CSS is expected to behave.</li>
<li> Because gradients are still supported in some browsers with prefixes and some not, and some with a slightly older syntax, you should use multiple background gradient properties with different syntaxes, as shown in the below examples."</li></ul>
<p><br />
</p>
<h3><span class="mw-headline" id="Related_specifications">Related specifications</span></h3>
<p>enter the most current specification the property is included in, AND the recommendation the property was included in, in the case of old properties that were included in CSS 1, 2.1, etc.
</p><p>For example:
</p><p>Name: CSS 2.1
URL: <a rel="nofollow" class="external free" href="http://www.w3.org/TR/CSS21/colors">http://www.w3.org/TR/CSS21/colors</a>
Status: W3C Recommendation
Relevant changes: 
</p><p>Name: CSS Backgrounds and Borders Module Level 3
URL: <a rel="nofollow" class="external free" href="http://www.w3.org/TR/css3-background/">http://www.w3.org/TR/css3-background/</a>
Status: W3C Candidate Recommendation
Relevant changes: Multiple background images can be specified on the same element.
</p><p><br />
</p>
<h3><span class="mw-headline" id="Compatibility_table">Compatibility table</span></h3>
<p>You can ignore the compatibility table for now. (We're working on brining in the data manually.) Update the compatibility notes field only if you think it's unique and isn't represented on sites like caniuse.com or developer.mozilla.org.
</p>
<h3><span class="mw-headline" id="Compatibility_notes">Compatibility notes</span></h3>
<p>Use the compatibility notes section to enter any useful specifics you have relating to browser compatibility. For example:
</p>
<ul><li> IE &lt; 9: doesn't support SVG for background-images, or multiple background images, or gradients</li>
<li> IE &lt; 10: doesn't support gradients</li>
<li> Not all browsers support animation of background images. Recent -webkit- based browsers transition between background images by cross fading.</li></ul>
<h3><span class="mw-headline" id="Related_articles">Related articles</span></h3>
<p>For the related articles, you should a include a wide variety of resources that nicely complement the subject in hand. You should choose:
</p>
<ul><li> Other reference articles covering properties (and subjects) related to this one</li>
<li> Tutorial articles that show how to use the property in more detail</li>
<li> Articles that contain interesting discussions related to the property, which might be of controversial or otherwise interesting nature</li>
<li> links to the spec(s) that the property appears in</li></ul>
<p>Here's some examples for the background-image example:
</p>
<h4><span class="mw-headline" id="Internal_pages_.28put_in_the_manual_links.27_section.29">Internal pages (put in the <i>manual links'</i> section)</span></h4>
<ul><li> <a href="/wiki/tutorials/using_css_background_images" title="tutorials/using css background images">Using CSS background images</a></li>
<li> <a href="/wiki/tutorials/creating_gradients_in_css" title="tutorials/creating gradients in css">Creating gradients in CSS</a></li></ul>
<h4><span class="mw-headline" id="Useful_external_articles_.28put_in_the_external_links_section.29">Useful external articles (put in the <b>external links</b> section)</span></h4>
<ul><li> <a rel="nofollow" class="external text" href="http://www.netmagazine.com/tutorials/get-grips-css3-multiple-background-images">Get to grips with CSS3 multiple background images</a>, by Prisca Schmarsow</li></ul>
<h3><span class="mw-headline" id="Anything_else_.28put_in_the_Manual_sections_section.29.3D">Anything else (put in the <b>Manual sections</b> section)=</span></h3>
<ul><li> x</li>
<li> y</li>
<li> z</li></ul>
<h3><span class="mw-headline" id="External_attribution">External attribution</span></h3>
<p>Some of the existing pages will have content that comes from an external source. We are quite happy to overwrite/replace this information, to improve it, make it more consistent, and get rid of any licensing constraints that using that material brought with it. If there is external attribution specified, and you've just rewritten the page data. uncheck the external attribution options.
</p>
<div class="attribution">
<p><br />
</p><p><br />
</p>
</div>

<!-- 
NewPP limit report
CPU time usage: 0.089 seconds
Real time usage: 0.109 seconds
Preprocessor visited node count: 217/1000000
Preprocessor generated node count: 960/1000000
Post‐expand include size: 508/2097152 bytes
Template argument size: 527/2097152 bytes
Highest expansion depth: 4/40
Expensive parser function count: 0/100
-->

<!-- 
Transclusion expansion time report (%,ms,calls,template)
100.00%   57.345      1 - -total
 25.76%   14.771      1 - Template:Page_Title
 19.08%   10.941      1 - Template:Flags
 15.39%    8.824      1 - Template:External_Attribution
 11.44%    6.562      1 - Template:Summary_Section
  8.22%    4.715      1 - Template:Notes_Section
  6.79%    3.896      1 - Template:Topics
  5.63%    3.229      1 - Template:Basic_Page
-->

<!-- Saved in parser cache with key wpwiki:pcache:idhash:7288-0!*!0!!*!*!*!esi=1 and timestamp 20150731045435 and revision id 34691
 -->
