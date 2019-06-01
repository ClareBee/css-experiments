---
layout: post
title:  "Continuous Image Border"
date:   2019-05-31 12:00:00 +0000
categories: jekyll css
---
<div class="default-grid border-frame">
 Continuous image as a border example
</div>

```css
.border-frame {
  padding: 2em;
  border: 2em solid transparent;
  background: linear-gradient(white, white) padding-box, url(../img/image.jpg) border-box 0 /cover;
}
```

Using white background to cover image background - with white added by a linear-gradient, since only the last layer can have a background-color.
Default background-origin is padding-box, so needs to be set to border-box.

<div class="default-grid gradient-pattern">
 using repeating-linear-gradient
</div>

<div class="default-grid marching-ants">
 using repeating-linear-gradient & keyframes
</div>

<div class="footnote">
  <sup>1</sup> This is a footnote.
</div>


Background shorthand =
`background: bg-color bg-image position/bg-size bg-repeat bg-origin bg-clip bg-attachment initial|inherit;`

*Note:* If one of the properties in the shorthand declaration is the bg-size property, you must use a / (slash) to separate it from the bg-position property, e.g. background:url(smiley.gif) 10px 20px/50px 50px; will result in a background image, positioned 10 pixels from the left, 20 pixels from the top, and the size of the image will be 50 pixels wide and 50 pixels high.

*Note:* If using multiple background-image sources but also want a background-color, the background-color parameter needs to be last in the list.

### Definitions
- *background-clip* = sets whether an element's background extends underneath its border box, padding box, or content box.
- *background-color*
- *background-image* = sets one or more background images on an element.
- *background-origin* =  sets the background's origin: from the border start, inside the border, or inside the padding. (ignored if background-attachment is fixed)
- *background-position* = sets the initial position for each background image. The position is relative to the position layer set by background-origin.
- *background-repeat* = sets how background images are repeated. A background image can be repeated along the horizontal and vertical axes, or not repeated at all.
- *background-size* = sets the size of the element's background image. The image can be left to its natural size, stretched, or constrained to fit the available space.
- *background-attachment* = sets whether a background image's position is fixed within the viewport, or scrolls with its containing block.
