---
layout: post
title:  "Pseudo-Random Backgrounds"
date:   2019-05-30 12:00:00 +0000
description: 'Illusion of randomness and the Cicada Principle'
categories: CSS
---
<div class="default-grid random-pattern">
</div>
<!--more-->
{% highlight css %}
.random-pattern {
  background: hsl(20, 40%, 90%);
  background-image:
    linear-gradient(90deg, #7A306C 11px, transparent 0),
    linear-gradient(90deg, #8E8DBE 23px, transparent 0),
    linear-gradient(90deg, #A9E4EF 41px, transparent 0);
  background-size: 41px 100%, 61px 100%, 83px 100%;
}
{% endhighlight %}
