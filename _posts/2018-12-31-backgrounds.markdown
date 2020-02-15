---
layout: post
title:  "CSS Backgrounds"
date:   2018-12-31 13:04:50 +0000
description: 'Flexible background positioning and stripes'
categories: CSS
---
<div class="flexible-background">
  <div>
    <p>Flexible background positioning with 'background-position' specifying offsets.</p>
    <p>Use 'bottom right' in background shorthand as fallback.</p>
    <p>Default positioning is relative to the padding box (not the border box or content box).</p>
    <p>Can be changed using 'background-origin'.</p>
  </div>
</div>
<!--more-->

<hr />
<div class="flexible-background-calc">
  <div>
    <p>Flexible background positioning with 'background-position' and 'calc()' specifying offsets from top left.</p>
  </div>
</div>
<hr />
<div class="inner-rounding">
  <div>
    <p>Simple inner rounding using 2 div elements</p>
  </div>
</div>
<hr />
<div class="inner-rounding-box">
  <p>Inner rounding using only 1 div element.</p>
  <p>'box-shadow' (no offsets, no blur) has rounding therefore covers gaps left by square-cornered 'outline'</p>
</div>
<hr />
<div class="container">
  <div class="striped-background">
    <div>
      <p>Striped background using linear-gradient using colour-stops with same position.</p>
    </div>
  </div>
  <div class="striped-background-2">
    <div>
      <p>Changing size of stripes using background-size and default repeat of gradient as background-image.</p>
    </div>
  </div>
  <div class="striped-background-3">
    <div>
      <p>Unequal width by changing color-stop size </p>
      <p>Setting second colour stop to 0 means browser will set it to the previous one.</p>
    </div>
  </div>
  <div class="striped-background-4">
    <div>
      <p>Three colours using extra values in linear-gradient.</p>
    </div>
  </div>
  <div class="striped-background-5">
    <div>
      <p>Vertical stripes using gradient direction 'to right' (defaults to 'to bottom').</p>
    </div>
  </div>
  <div class="striped-background-6">
    <div>
      <p>Diagonal stripes using gradient direction of '45deg', color stops, repeating tile.</p>
    </div>
  </div>
  <div class="striped-background-7">
    <div>
      <p>Easier diagonal stripes using 'repeating-linear-gradient()'.</p>
    </div>
  </div>
  <div class="striped-background-8">
    <div>
      <p>Using 'repeating-linear-gradient()' for stripes with adjustable angle.</p>
    </div>
  </div>
  <div class="striped-background-9">
    <div>
      <p>Flexible subtle stripes by using background colour and hsla and transparent.</p>
    </div>
  </div>
</div>