---
layout: post
title:  "Cutout Corners"
date:   2019-06-05 12:00:00 +0000
description: 'Linear gradients and colour stops'
categories: CSS
---

<div class="cutout-corner"></div>
<br/>
{% highlight css %}
.cutout-corner {
  width: 100px;
  height: 100px;
  background: #A9E4EF;
  background: linear-gradient(-45deg, transparent 15px, #A9E4EF 0);
}
{% endhighlight %}
<!--more-->

<p>Gradients can accept angle direction & colour stop positions in absolute lengths</p>
<div class="cutout-corners"></div>
<br />
{% highlight css %}
.cutout-corners {
  width: 100px;
  height: 100px;
  background: #A9E4EF;
  background:
      linear-gradient(135deg, transparent 15px, #A9E4EF 0) top left,
      linear-gradient(-135deg, transparent 15px, #A9E4EF 0) top right,
      linear-gradient(-45deg, transparent 15px, #A9E4EF 0) bottom right,
      linear-gradient(45deg, transparent 15px, #A9E4EF 0) bottom left;
  background-size: 50% 50%;
  background-repeat: no-repeat;
}
{% endhighlight %}
<p>All four corners using linear-gradients with appropriate degree angles, transparent colour stops and position</p>
<div class="curved-cutout-corners"></div>
<p>Curved corners using radial-gradient + transparent circles at each corner</p>

{% highlight css %}
.curved-cutout-corners {
  width: 200px;
  height: 100px;
  background: #8E8DBE;
  background:
      radial-gradient(circle at top left, transparent 15px, #8E8DBE 0) top left,
      radial-gradient(circle at top right, transparent 15px, #8E8DBE 0) top right,
      radial-gradient(circle at bottom right, transparent 15px, #8E8DBE 0) bottom right,
      radial-gradient(circle at bottom left, transparent 15px, #8E8DBE 0) bottom left;
  background-size: 50% 50%;
  background-repeat: no-repeat;
}
{% endhighlight %}

<p>CSS Backgrounds & Borders Level 4 will bring 'corner-shape'</p>
