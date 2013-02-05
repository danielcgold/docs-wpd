{{Page_Title}}
{{Flags}}
{{Standardization_Status|W3C Recommendation}}
{{API_Name}}
{{Summary_Section|Specifies the size of text. Sets the font size of the element to which it is applied, and its descendants. Can size text using absolute measurements, or relative to the parent or root elements. [[guides/css_text_styling_fundamentals|CSS Text Styling Fundamentals]] provides an overview.}}
{{CSS Property
|Initial value=medium
|Applies to=All elements
|Inherited=Yes
|Media=visual
|Computed value=absolute size in '''px''' units
|Animatable=Yes
|CSS object model property=fontSize
|CSS percentages=???
|Values={{CSS Property Value
|Data Type=absolute-size
|Description=A set of keywords indicating predefined font sizes that scale according to font setting preferences or each browser's default values. From small to large, possible values are '''xx-small''', '''x-small''', '''small''', '''medium''', '''large''', '''x-large''', and '''xx-large'''.
}}{{CSS Property Value
|Data Type=relative-size
|Description=A set of keywords interpreted relative to the parent element's '''font-size''', either '''smaller''' or '''larger'''.
}}{{CSS Property Value
|Data Type=length
|Description=A positive numeric value followed by a string designating [[css/units/length|absolute or relative units of length]]. Proportional [[css/units/length|'''em''' and '''ex''']] measurements are based on the parent element's '''font-size''', while [[css/units/length|'''rem''']] measurements are based on that of the root element.
}}{{CSS Property Value
|Data Type=percentage
|Description=A positive integer followed by a percent ([[css/units/numeric|'''%''']]), indicating the proportion of the parent element's '''font-size'''.
}}
}}
{{Examples_Section
|Not_required=No
|Examples={{Single Example
|Language=CSS
|Description=Redefine the typical '''16px''' default '''medium''' value as '''10px''', then redefine other tags in proportion to the root:
|Code=html { font-size: 62.5%; } /* 16 * 62.5% == 10 */

h1 { font-size: 3.6rem }   /* 36px */
h2 { font-size: 2.4rem }   /* 24px */
p  { font-size: 1.4rem }   /* 14px */
}}{{Single Example
|Language=HTML
|Description=The interactive utility demonstrates absolute values applied to a block of text, and relative values applied to the first sentence.
|Code=See live example above.
|LiveURL=http://letmespellitoutforyou.com/x/webplatform/fontSize.html
}}
}}
{{Notes_Section
|Usage=Keywords such as '''large''' and '''medium''', or relative '''em''' or percentage units, are generally safer to use than pixel measurements, especially for mobile web browsers that adjust their set of default font sizes for legibility. Otherwise, pixels offer the safest way to specify measurements, since [[css/concepts/CSS_pixels|CSS pixels]] are adjusted for variations in display pixel density.

While the initial '''medium''' size applies widely, browsers apply a default style sheet that modifies it for various semantic elements, boosting the size of headings, for example. Browsers also automatically resize fonts when zooming the page, stepping by values that may not correspond exactly to the zoom factor. Unless disabled using [[css/properties/text-size-adjust|'''text-size-adjust''']], fonts also resize when tipping between portrait and landscape orientations on mobile browsers. For an overview of the issue, see [[tutorials/mobile_viewport|The Mobile Viewport and Orientation]].

The value of '''font-size''' also affects the value of [[css/properties/line-height|'''line-height''']] when using its default or relative measurements.

Along with many other CSS properties, '''font-size''' can also be applied directly as an SVG attribute:

<syntaxhighlight lang="xml">
<text x="12px" y="12px" font-family="sans-serif" font-size="120%"/>
</syntaxhighlight>
}}
{{Related_Specifications_Section
|Specifications={{Related Specification
|Name=CSS Fonts Module Level 3
|URL=http://www.w3.org/TR/css3-fonts/#font-size-prop
|Status=Working Draft
}}{{Related Specification
|Name=CSS Values and Units Module Level 3
|URL=http://www.w3.org/TR/css3-values/
|Status=Candidate Recommendation
}}
}}
{{Compatibility_Section
|Not_required=No
|Imported_tables=
|Desktop_rows={{Compatibility Table Desktop Row
|Chrome_supported=Yes
|Chrome_version=1.0
|Chrome_prefixed_supported=No
|Chrome_prefixed_version=
|Firefox_supported=Yes
|Firefox_version=1.0
|Firefox_prefixed_supported=No
|Firefox_prefixed_version=
|Internet_explorer_supported=Yes
|Internet_explorer_version=5.5
|Internet_explorer_prefixed_supported=No
|Internet_explorer_prefixed_version=
|Opera_supported=Yes
|Opera_version=7.0
|Opera_prefixed_supported=No
|Opera_prefixed_version=
|Safari_supported=Yes
|Safari_version=1.0
|Safari_prefixed_supported=No
|Safari_prefixed_version=
}}
|Mobile_rows={{Compatibility Table Mobile Row
|Android_supported=Yes
|Android_version=1.0
|Android_prefixed_supported=No
|Android_prefixed_version=
|Blackberry_supported=Yes
|Blackberry_version=3.8
|Blackberry_prefixed_supported=No
|Blackberry_prefixed_version=
|Chrome_mobile_supported=Yes
|Chrome_mobile_version=1.0
|Chrome_mobile_prefixed_supported=No
|Chrome_mobile_prefixed_version=
|Firefox_mobile_supported=Yes
|Firefox_mobile_version=1.0
|Firefox_mobile_prefixed_supported=No
|Firefox_mobile_prefixed_version=
|IE_mobile_supported=Yes
|IE_mobile_version=6.0
|IE_mobile_prefixed_supported=No
|IE_mobile_prefixed_version=
|Opera_mobile_supported=Yes
|Opera_mobile_version=6.0
|Opera_mobile_prefixed_supported=No
|Opera_mobile_prefixed_version=
|Opera_mini_supported=Yes
|Opera_mini_version=1.0
|Opera_mini_prefixed_supported=No
|Opera_mini_prefixed_version=
|Safari_mobile_supported=Yes
|Safari_mobile_version=1.0
|Safari_mobile_prefixed_supported=No
|Safari_mobile_prefixed_version=
}}
|Notes_rows={{Compatibility Notes Row
|Browser=IE
|Version=≤ 6.0
|Note=Requires a [[html/elements/!DOCTYPE|'''!DOCTYPE''']] declaration that triggers [[concepts/standards_mode|standards mode]], otherwise the initial value is '''small''' rather than '''medium'''.
}}{{Compatibility Notes Row
|Browser=IE
|Version=≤ 7.0
|Note=Does not support '''inherit''' as a value.
}}{{Compatibility Notes Row
|Browser=IE
|Version=≤ 8.0
|Note=Does not resize text specified with absolute pixel measurements when using the browser's ''text-resize'' feature, but does resize correctly when zooming the page.
}}{{Compatibility Notes Row
|Browser=IE
|Version=≤ 8.0
|Note=Does not support [[css/units/length|'''rem''']] values; specify other supported values as fallback properties.
}}{{Compatibility Notes Row
|Browser=All
|Note=Check compatibility for more recent [[css/units/length|viewport unit values]].
}}
}}
{{See_Also_Section
|Topic_clusters=CSS Font, Fonts, Text
|External_links=* Smashing: [http://www.smashingmagazine.com/2011/10/07/16-pixels-body-copy-anything-less-costly-mistake 16 Pixels: For Body Copy. Anything Less Is a Costly Mistake]
* HTML5 Boilerplate: [https://github.com/h5bp/html5-boilerplate/issues/724 Reasoning behind default font-size and line-height]
* A List Apart: [http://www.alistapart.com/articles/howtosizetextincss How to Size Text in CSS]
* Mozilla: [http://mxr.mozilla.org/mozilla/source/layout/style/html.css default style sheet]
* WebKit: [http://trac.webkit.org/browser/trunk/Source/WebCore/css/html.css default style sheet]
}}
{{Topics|CSS}}
{{External_Attribution
|Is_CC-BY-SA=No
|MDN_link=
|MSDN_link=
|HTML5Rocks_link=
}}