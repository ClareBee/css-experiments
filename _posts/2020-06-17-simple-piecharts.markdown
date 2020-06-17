---
layout: post
title: "Pie Charts"
date: 2020-06-17 12:00:00 +0000
description: "Transform and SVG solutions"
categories: CSS
---

### Transform-based pie charts

- using pseudo-elements, transforms, CSS gradients
<!--more-->

<div class="pie-chart"></div>

- using a rotating pseudo-element `::before` with same colour as background to uncover only the percentage needed (using overflow hidden to fit the shape)
- possible to customise this to be a set percentage using negative animation delay on inline style => pauses it
- i.e. the % shown on the pie chart = the % of the total duration our animation delay is

```css
.pie-chart {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  background: $brand-color;
  background-image: linear-gradient(to right, transparent 50%, #655 0);
}

.pie-chart::before {
  content: "";
  display: block;
  margin-left: 50%;
  height: 100%;
  border-radius: 0 100% 100% 0 / 50%;
  background-color: inherit;
  transform-origin: left;
  transform: rotate(0.1turn);
  animation: spin 3s linear infinite, bg 6s step-end infinite;
}

@keyframes spin {
  to {
    transform: rotate(0.5turn);
  }
}

@keyframes bg {
  50% {
    background: #655;
  }
}
```

### SVG-based pie charts

- using stroke-dasharray => width & gap can be set so that stroke covers radius of our circle

```html
<svg class="pie" width="100" height="100">
  <circle r="25" cx="50" cy="50" />
</svg>
```

<svg class="pie" width="100" height="100">
<circle r="25" cx="50" cy="50" />
</svg>
