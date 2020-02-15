---
layout: post
title:  "Trapezoid Tabs"
date:   2019-06-08 12:00:00 +0000
description: 'ScaleY, perspective and rotate'
categories: CSS
---
<div class="trapezoid">Trapezoid</div>
<!--more-->

<p>Trapezoid using transform with scaleY, perspective & rotate with a pseudo-element</p>

{% highlight css %}
.trapezoid {
  position: relative;
  display: inline-block;
  padding: .5em 1em .35em;
  color: white;
  text-align: center;
}
.trapezoid::before {
  content: '';  /* to generate the box */
  position: absolute;
  top: 0; right: 0; bottom: 0; left: 0;
  z-index: -1;
  background: #8E8DBE;
  transform: scaleY(1.3) perspective(.5em) rotateX(5deg);
  transform-origin: bottom; /* so base remains fixed as it rotates in space */
}
{% endhighlight %}

<p>Lea Verou's styled tabs</p>

<nav class="nav left">
	<a href="#">Home</a>
	<a href="#" class="selected">Projects</a>
	<a href="#">About</a>
</nav>
<main class="content">
	Content area
</main>
