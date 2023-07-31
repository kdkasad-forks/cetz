* 0.0.2
** Content
- The `content` function now supports a second coordinate as `angle`, to
  compute the rotation angle between the origin
- *[!]* Anchors of the `content` function are now properly rotated

** Tree
- Added the `tree` module for laying out trees

** Canvas
- *[!]* Changed transformation matrix multiplication order from `Local * World to`
  World * Local.
- Added `set-viewport` function for setting up scaling and translation to draw
  insides a rectangular region
- *[!]* The function `rect` now emits rotated anchors,
  before it did not set anchors but used the bounding box
- New function `copy-anchors` to copy anchors of an element into a group
- Arcs are now approximated using up to 4 bezier curves instead of using
  sampling with straight lines

** Chart
- Added new library `chart` for drawing charts, currently only bar- and columncharts are supported

** Plot
- Added new library `plot` for drawing line charts (of functions), replacing `typst-plot`