> The contents here is created from the official [CascadiaJS Page](https://2022.cascadiajs.com/speakers/chris-coyier)

## Overview

![Chris Coyier image](https://create-4jr.begin.app/_static/2022/chris-coyier.jpg){max-width: 300px}
- name: Chris Coyier
- [Speaker Page](https://2022.cascadiajs.com/speakers/chris-coyier)

## Abstract

There are quite a few things in the world of web design and development that have gotten… easy. It might be time to take a look at how you’re approaching some of the building blocks of your website because evolutions in browser technology and tooling have made many things easier and better. We’ll have a look at browser-level things like things as fundamental as layout, typography, and animation. Then also tooling level things like media handling, serverless concepts, and hosting.

## Notes


### Hunter's notes


- Chris Coyier
  - Has published 5k blog posts.
  - Runs the shop talk podcast?
- Ate every breakfast burrito in Bend.
- took pictures, entered data...
- Used Astro to build his website.
- "CSS Scripture"
	- Grid layout is great for sorting cards.
		- As many as fit ===repeaaat(auto-fit, minmax(min(100%,360px), fr));
		- grid-template-columns: masonry
	- Container queries are a new thing on the way
		- can style a component against its own container.
		- uses wrapper divs
		- `@container <name <size> { // style }`
	- WAAPI Web Animation API
		- `element.animate(ary, opts)`
		- Maybe you don't need an animation framework anymore
	- Scroll timelines is a thing that might be coming soon... define scroll events with keyframes.
	- `offset-path` and `offsite-distance` to animate with apath.
		- This one, comes in on a curve.  *laugh*
	- FLIP.... too fast to take notes
		- Can chsange the order of elements with css...?
	- Web typography
		- woff2 file `@font-face{ src: url(/fonts/roboto.woff2)\nformat('woff2');...}`
		- You can control how a custom font loads...  `font-display: swap`
			- This should be used for most sites so that content doesn't have a delayed load.
			- Can use `optional` instead of `swap` to prevent flicker (and loading of font).
			- `system-ui` is a proper font-family
		- Fonts can have `font-variation-settings` kind of like shaders in rendering engines.
	- Fluid type "is how you should do typography on the web".
		- express a formula for setting font size and stuff without making concrete breakpoints?
		- `clamp`
		- Very cool way of doing typography.
	- Image son the web these days need multpile sources and stuff for different screen sizes.
		- Lots of considerations with images
		- Cloudinary handles images.  $
			- can use canonical image
		- use `srcset` with `sizes` attributes on an image.
		- Other tools with cloudinary
			-imgix and codepen (another one shown)...
	- "Browsers are sneaky bastards", they should abide by standards, the web is good as long as people are vigilant.
