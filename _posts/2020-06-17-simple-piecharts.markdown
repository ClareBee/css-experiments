---
layout: post
title: "Pie Charts"
date: 2020-06-17 12:00:00 +0000
description: "Transform and SVG solutions"
categories: CSS
---

## Piecharts

### Transform-based pie charts

- using pseudo-elements, transforms, CSS gradients
<!--more-->

<div class="pie-chart"></div>

- using a rotating pseudo-element `::before` with same colour as background to uncover only the percentage needed (using overflow hidden to fit the shape)
- possible to customise this to be a set percentage using negative animation delay on inline style => pauses it
- i.e. the % shown on the pie chart = the % of the total duration our animation delay is

### SVG-based pie charts

- using stroke-dasharray => width & gap can be set so that stroke covers radius of our circle

<svg class="pie" width="100" height="100">
<circle r="25" cx="50" cy="50" />
</svg>
