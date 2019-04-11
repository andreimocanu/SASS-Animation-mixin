# SASS Animation mixin

An easy to use mixin for generating animation css.

<h3>Usage</h3>

<pre>
// Default settings
.element1 {
  @include anim();
}

// Disable animation
.element2 {
  @include anim(none);
}

// 0.1s animation duration
.element3 {
  @include anim(0.1s);
}

// 0.1s animation duration and linear transition timing
.element4 {
  @include anim(0.2s, linear);
}
</pre>

<h3>Result</h3>

<pre>
.element1 {
  -webkit-transition: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
}

.element2 {
  -webkit-transition: none;
  transition: none;
}

.element3 {
  -webkit-transition: all 0.1s ease-in-out;
  transition: all 0.1s ease-in-out;
}

.element4 {
  -webkit-transition: all 0.2s linear;
  transition: all 0.2s linear;
}
</pre>
