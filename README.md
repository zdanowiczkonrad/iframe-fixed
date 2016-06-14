# Iframe overflow scrolling with `position: fixed;`

This demo includes cross-browser samples of `iframe` elements that have `position: fixed` (ie. overlay modal with iframe content) and has scrollable contents _(iframe's content height is larger than the parent document height)_.

For most browser this is a no-brainer, but iOS Safari does not simply render iframe's overflow - it renders iframe's overflow as `visible` without possibility to change it and the scroll events are bubbled under the iframe, to the document body usually, which is something you usually don't desire.


## Compatibility
This code solves issues mentioned above and works almost identically for following browsers:

### Desktop

	* Chrome 51.0.2704.84
	* Firefox 47.0
	* Safari 9.1 (11601.5.17.1)
	* MS Edge (25.10586.0.0)
	* IE 11 (11.0.31) 

### Mobile

	* iOS Safari 9.3 (13E230)
	* Chrome 50.0.266.89


## Demos

* [Fullscreen iframe overlay with position: fixed + defined iframe's height](01-fullscreen.html)
* [Fullscreen iframe overlay with position: fixed + undefined iframe's height](02-fullscreen-no-height.html)
* [Fullscreen iframe overlay with position: fixed + infinite scroll](03-infiniscroll.html)

