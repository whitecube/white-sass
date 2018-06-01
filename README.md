white-sass
==========

A few SASS mixins and functions we use on daily basis

## Update 05/02/2018

Reworked some of the font helpers and added a color mixin.

**Fonts & Sizing**  

### `font(family, variant)`  
Adds the necessary css rules to use the requested font/variant combo. These values are defined beforehand in the `$ws_fonts-path` variable (`config/_fonts.scss`)

### `em(goal, parent)`  
Returns a `em` value for the given parameters, which can either be a font-size identifier (defined in `config/_typography`) or a numeric value (expressed in pixels).

### `px(goal)`  
Returns a `px` value for the given parameters, which can either be a font-size identifier (defined in `config/_typography`) or a numeric value (expressed in pixels).

### `fvalue(font-size)`  
Returns an unit-less pixel value for the given font-size identifier (defined in `config/_typography`).

**Colors**  
### `color(color)`  
Returns the color code defined in the `$ws_colors` variable (`config/_colors.scss`)

## Update 11/12/2015

Added **Kaduk**, a mixin (using independent functions if you want more flexibility) that allows you to do this (and it works in responsive if you pass it a percentage value) :

![schema of Kaduk ](https://raw.githubusercontent.com/whiteCube/white-sass/master/kaduk.png)

## Update 11/11/2015

Added the following features :

- Gridz: `fixedCol()`: You can now get grid values returned in `px`, `em`, `rem` or `bananas` instead of `%`.
- Utils:
      - `cover()`: Set an element's position in order to cover its relative parent.
      - `rmUnit()`: Removes units from values (Different from Sass's `unitless()`, which only returns `true` or `false`)
      - `clickableTransparentBg()`: Easy bug fix for IE on transparent links displayed as blocks.
- Sprites: `@include setHalfSpriteBack()`: does exactly what it says
- **Icons !** You can now easily use icon-fonts and add pink SVG hearts everywhere with a simple mixin !


Updated :

- Config file is now easier to use.
- pseudoElements: triangles can now be used on any element (but it's always better on a `::before` or `::after`) and has all the possible directions (topLeft, top, topRight, right, bottomRight, bottom, bottomLeft, left).
- Sprites: added retina support (we actually used it for a while but never added it to this repo).

Removed :

- CompassOverride. Was not pertinent anymore.