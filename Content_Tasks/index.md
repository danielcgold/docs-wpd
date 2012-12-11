A list of required actions in the long run, mostly due to the fact that the current templates do not support certain scenarios.
*Add compatibility tables, unless automation effort gets the right information -
**[[dom/methods/hasAttribute]]
*Remove "Non standard" from the summary once there is an automatic indication in the listing pages (non exhaustive, unfortunately) -
**[[dom/traversal/methods/queryCommandText]]
**[[dom/traversal/methods/expand]]
**[[dom/methods/navigate]]
**[[dom/methods/cancelBubble]]
**[[dom/methods/ChooseColorDlg]]
**[[dom/properties/canHaveChildren]]
**[[dom/properties/compatible]]
**[[dom/ClipboardData]]
**[[dom/methods/getAttribute_(userProfile)]]
**[[dom/methods/dragDrop]]
**[[dom/properties/cpuClass]]
**[[dom/userProfile]]
**[[dom/methods/createPopup]]
**[[dom/properties/srcElement]]
**[[dom/properties/reason2]]
**[[dom/properties/which]]
**[[dom/properties/x (mouseevent)]]
**[[dom/properties/y (mouseevent)]]
**[[dom/properties/boundElements]]
**[[dom/methods/releaseCapture]]
**[[dom/properties/returnValue]]
**[[dom/properties/fromElement]]
**[[dom/methods/setCapture]]
**[[dom/methods/fireEvent]]
**[[dom/methods/applyElement]]
**[[dom/properties/browserLanguage]]
*Miscellaneous -
**[[dom/methods/getElementsByTagNameNS]] - change the return type to HTMLCollection or whatever.
**[[dom/methods/getAttribute_(userProfile)]], [[dom/properties/cpuClass]], [[dom/userProfile]] - apply to [[dom/Navigator]] when it exists
**[[cssom/ClientRect]] - needs further work?
**[[dom/methods/replaceState]] - explain the buggy behavior of Safari 5 and later.
**[[Template:API_Object_Property_New]] - work in progress.
**[[dom/properties/reason2]] - find the event that uses this property.
**[[dom/methods/cancelBubble]] - should probably be removed.
**[[dom/objects/dataTransfer]] - change its URL to be property related one or something (?).
**[[dom/ClipboardData]] - needs an offer for an alternative, standard (track) implementation (event.dataTransfer?)
**[[dom/properties/defaultValue]] should link to the value HTML attribute. A page for which does not seem to exist.
*Needs support for multiple values in the "Applies to..." field -
{|
! Page
! Future Multiple "Applies to..." Values
|-
|[[dom/methods/getElementsByTagName]]
|[[dom/Document]], [[dom/HTMLElement]]
|-
|[[dom/methods/getElementsByTagNameNS]]
|[[dom/Document]], [[dom/Element]]
|-
|[[css/selectors_api/querySelectorAll]]
|[[dom/Document]], [[dom/HTMLElement]]
|-
|[[css/selectors_api/querySelector]]
|[[dom/Document]], [[dom/HTMLElement]]
|-
|[[dom/methods/attachEvent]]
|[[dom/Document]], [[dom/Window]], [[dom/Node]]
|-
|[[dom/properties/complete]]
|[[dom/HTMLImageElement]], [[dom/images|dom/Image]](?), [[dom/HTMLInputElement|dom/HTMLInputElement type=image]]
|-
|[[dom/methods/getModifierState]]
|[[dom/objects/KeyboardEvent]],
[[dom/objects/MouseEvent]], more?
|-
|[[dom/properties/fgColor]]
|[[dom/Document]], [[dom/HTMLBodyElement]]
|-
|[[dom/methods/releaseCapture]]
|[[dom/Document]], [[dom/Element]]
|-
|[[dom/methods/setData]], [[dom/methods/getData]], [[dom/methods/clearData]]
|[[dom/objects/dataTransfer]], [[dom/ClipboardData]]
|-
|[[apis/file/methods/abort]]
|[[apis/file/FileReader]], [[apis/file/MSStreamReader]]
|-
|[[apis/audio-video/events/addtrack]]
|[[apis/audio-video/TextTrackList]]
|-
|[[dom/traversal/properties/filter]]
|[[dom/traversal/TreeWalker]] and the current one
|-
|[[dom/properties/data]]
|[[dom/objects/CompositionEvent|CompositionEvent]], [[dom/objects/MessageEvent|MessageEvent]], [[dom/objects/TextEvent|TextEvent]]
|-
|[[dom/properties/locale]]
|[[dom/objects/CompositionEvent|CompositionEvent]], [[dom/objects/KeyboardEvent|KeyboardEvent]], [[dom/objects/TextEvent|TextEvent]]
|}
*Pages on which a lot of pages depend that should be moved/renamed -
{|
! Page
! Move/Rename To
|-
|[[dom/images]]
|[[dom/Image]] (?!)
|-
|[[dom/properties/children_(document)%2BB416]]
|[[dom/properties/children]]
|-
|[[concepts/programming/javascript/objects/js/objects/Object/getOwnPropertyNames]]
|[[javascript/Object/getOwnPropertyNames]]
|}