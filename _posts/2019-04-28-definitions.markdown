---
layout: post
title:  "CSS Linear and Radial Gradients"
date:   2019-04-28 12:00:00 +0000
description: 'Definition of linear and radial gradients'
categories: CSS
---
<div class="flex-container">
  <div class="default-grid linear-example">
  </div>

{% highlight css %}
.linear-example {
  background-image: linear-gradient(90deg, #A9E4EF, #8E8DBE 15%);
  background-size: 30px;
  background-position: center;
}
{% endhighlight %}

  <div class="default-grid radial-example">
  </div>

{% highlight css %}
.radial-example {
  background-image:
    radial-gradient(circle at center, #7A306C 0, #8E8DBE, #A9E4EF 100%);
}
{% endhighlight %}  
</div>
<!--more-->

<blockquote>
  The linear-gradient() CSS function creates an image consisting of a progressive transition between two or more colors along a straight line. Its result is an object of the gradient data type, which is a special kind of image.
  A linear gradient is defined by an axis—the gradient line—and two or more color-stop points. Each point on the axis is a distinct color; to create a smooth gradient, the linear-gradient() function draws a series of colored lines perpendicular to the gradient line, each one matching the color of the point where it intersects the gradient line.
</blockquote>

<caption>From MDN</caption>
<hr>
<strong>background-image: linear-gradient(direction, color-stop1, color-stop2, ...);</strong>

<strong>background-image: radial-gradient(shape size at position, start-color, ..., last-color);</strong>
