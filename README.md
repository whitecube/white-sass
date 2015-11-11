white-sass
==========

A few SASS mixins and functions we use on daily basis

## Update 11/11/2015

Added the following features :

- Gridz
      - `fixedCol()`: You can now get grid values returned in `px`, `em`, `rem` or `bananas` instead of `%`.
- Utils
      - `rmUnit()`: Removes units from values (Different from Sass's `unitless()`, which only returns `true` or `false`)


Updated :

- Config file is now easier to use.
- pseudoElements: triangles can now be used on any element (but it's always better on a `::before` or `::after`) and has all the possible directions (topLeft, top, topRight, right, bottomRight, bottom, bottomLeft, left).
- Sprites: added retina support (we actually used it for a while but never added it to this repo).

Removed :

- CompassOverride. Was not pertinent anymore.