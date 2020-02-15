---
layout: post
title:  "CSS Backgrounds"
date:   2018-12-31 13:04:50 +0000
description: 'Stripes'
categories: CSS
---

<div class="inner-rounding">
  <div>
    <p>Simple inner rounding using 2 div elements</p>
  </div>
</div>
<br />
{% highlight css %}

.inner-rounding {
  width: 300px;
  margin: 0 auto;
  background: #8E8DBE;
  padding: .8em;
}

.inner-rounding > div {
  background: #A9E4EF;
  border-radius: .8em;
  padding: 1em;
}
{% endhighlight %}

<br />

<div class="inner-rounding-box">
  <p>Inner rounding using only 1 div element.</p>
  <p>'box-shadow' (no offsets, no blur) has rounding therefore covers gaps left by square-cornered 'outline'</p>
</div>
<br />

{% highlight css %}
.inner-rounding-box {
  width: 300px;
  margin: 0 auto;
  background: #A9E4EF;
  border-radius: .8em;
  padding: 1em;
  box-shadow: 0 0 0 .6em #8E8DBE;
  outline: .6em solid #8E8DBE;
}
{% endhighlight %}

<br />
<hr />
<br/>
<div class="container">
  <div class="striped-background">
    <div>
      <p>Striped background using linear-gradient using colour-stops with same position.</p>
    </div>
  </div>
{% highlight css %}
.striped-background {
  background: linear-gradient(#8E8DBE 50%, #A9E4EF 50%);
}
{% endhighlight %}
  <div class="striped-background-2">
    <div>
      <p>Changing size of stripes using background-size and default repeat of gradient as background-image.</p>
    </div>
  </div>
{% highlight css %}
.striped-background-2 {
  background: linear-gradient(#8E8DBE 50%, #A9E4EF 50%);
  background-size: 100% 30px;
}
{% endhighlight %}
  <div class="striped-background-3">
    <div>
      <p>Unequal width by changing color-stop size </p>
      <p>Setting second colour stop to 0 means browser will set it to the previous one.</p>
    </div>
  </div>
{% highlight css %}
.striped-background-3 {
  background: linear-gradient(#8E8DBE 30%, #A9E4EF 0);
  background-size: 100% 30px;
}
{% endhighlight %}
  <div class="striped-background-4">
    <div>
      <p>Three colours using extra values in linear-gradient.</p>
    </div>
  </div>
{% highlight css %}
.striped-background-4 {
  background: linear-gradient(#8E8DBE 30%, #A9E4EF 0, #A9E4EF 66.6%, #7A306C 0);
  background-size: 100% 45px;
}
{% endhighlight %}
  <div class="striped-background-5">
    <div>
      <p>Vertical stripes using gradient direction 'to right' (defaults to 'to bottom').</p>
    </div>
  </div>
{% highlight css %}
.striped-background-5 {
  background: linear-gradient(to right, #8E8DBE 30%, #A9E4EF 0, #A9E4EF 66.6%, #7A306C 0);
  background-size: 30px 100%;
}
{% endhighlight %}
  <div class="striped-background-6">
    <div>
      <p>Diagonal stripes using gradient direction of '45deg', color stops, repeating tile.</p>
    </div>
  </div>
{% highlight css %}
.striped-background-6 {
  background: linear-gradient(45deg, #8E8DBE 25%, #A9E4EF 0, #A9E4EF 50%, #8E8DBE 0, #8E8DBE 75%, #A9E4EF 0);
  background-size: 42px 42px;
}
{% endhighlight %}
  <div class="striped-background-7">
    <div>
      <p>Easier diagonal stripes using 'repeating-linear-gradient()'.</p>
    </div>
  </div>
{% highlight css %}
.striped-background-7 {
  background: repeating-linear-gradient(45deg, #8E8DBE, #A9E4EF 30px);
}
{% endhighlight %}
  <div class="striped-background-8">
    <div>
      <p>Using 'repeating-linear-gradient()' for stripes with adjustable angle.</p>
    </div>
  </div>
{% highlight css %}
.striped-background-8 {
  background: repeating-linear-gradient(25deg, #8E8DBE, #8E8DBE 15px,  #A9E4EF 0, #A9E4EF 30px);
}
{% endhighlight %}
  <div class="striped-background-9">
    <div>
      <p>Flexible subtle stripes by using background colour and hsla and transparent.</p>
    </div>
  </div>
{% highlight css %}
.striped-background-9 {
  background: #7A306C;
  background-image:
    repeating-linear-gradient(30deg, hsla(0, 0%, 100%, .1),
                                     hsla(0, 0%, 100%, .1) 15px,
                                    transparent 0, transparent 30px);
}
{% endhighlight %}
</div>
