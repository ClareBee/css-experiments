Hover States, Little Big Details, Dribble.

Wow.js, Animate.css, Hover.css, Modernizr
Accessibility eg Vestibular.org
NNGroup’s Animation for Attention and Comprehension
GSAP - Greensock Animation Platform
Snabbt.js

transitions don't work on font-family or background-images created w css (e.g. linear gradient)
they do work w opacity and positioning of background-images

Using JavaScript:
incl. vendor prefixes:
document.getElementById('js-show').style.webkitTransition = 'opacity 1s ease-out';
document.getElementById('js-show').style.transition = 'opacity 1s ease-out';

// animation
shorthand:
animation: change-background 4s linear infinite;
longhand:
animation-name: change-background;
animation-duration: 4s;
animation-timing-function: linear;
animation-repeat: infinite;

A set of keyframes in CSS is a series of stops along the way through an animation. Each “keyframe” is a written as a percentage.

//animation properties
+ animation-delay (doesn't apply in loops)
+ animation-direction: normal/reverse/alternate/alternate-reverse;
+ animation-duration: 1s/200ms;
+ animation-fill-mode: forwards (stays on last keyframe)/backwards (returns to first keyframe);
+ animation-iteration-count: 1/infinite;
+ animation-name: name of @keyframes;
+ animation-play-state: running(default)/paused;
+ animation-timing-function: applied between each keyframe;
