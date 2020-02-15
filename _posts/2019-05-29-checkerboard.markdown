---
layout: post
title:  "CSS Checkerboards Using Linear Gradients"
date:   2019-05-29 12:00:00 +0000
description: 'Basic checked patterns'
categories: CSS
---
<div class="flex-container">
  <div class="default-grid triangle-checkerboard">
  </div>
  <br />
  {% highlight css %}
  .triangle-checkerboard {
    background: #eee;
    background-image: linear-gradient(45deg, transparent 75%, #bbb 0);
    background-size: 30px 30px;
  }
  {% endhighlight %}
  <br />
  <div class="default-grid checkerboard">
  </div>
  <br />
  {% highlight css %}
  .checkerboard {
    background: #eee;
    background-image:
        linear-gradient(45deg, #bbb 25%, transparent 0),
        linear-gradient(45deg, transparent 75%, #bbb 0),
        linear-gradient(45deg, #bbb 25%, transparent 0),
        linear-gradient(45deg, transparent 75%, #bbb 0);
    background-position: 0 0, 15px 15px, 15px 15px, 30px 30px;
    background-size: 30px 30px;
  }

  {% endhighlight %}
</div>
<hr >
