Summary
=======================

Sass mixin that lets anyone easily implement an animated background gradient.


Usage
=======================

After you've included the SCSS file into your project you simply need to include it in the SCSCC for the element
you'd like to animate, like so:

__element {
  @include gradient-animation($direction, $duration, ($colors))
}__

The mixin takes three arguments:

_$direction:_ This is the direction of the linear animation, e.g., 125deg.
$duration: The total animation time in seconds, e.g., 40s. I recommend 30s+ for a smooth gradient.
$colors: This is a list of colors you'd like to include in the animation. Pass the list inside parantheses. 

Example
========================

element {
  @include gradient-animation(125deg, 50s, (#ff44ff, #aaff33, #33dd33, #33ff55));
}
