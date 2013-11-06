# noUiSlider

noUiSlider is lightweight plugin, developed to be a jQuery UI alternative. It features cross-browser support, a `just-another-input-type` style of getting and setting values, a wide range of options and support for a bunch of touch devices. It works wonders on Android phones, iPhone & iPad, Windows phone and touch-screen laptops and tablets. It works excellent on the desktop too; All modern browsers and IE7+ are supported. The end result? A lean, extendible and bloat-less plugin that'll just do its job. To add even more flexibility, noUiSlider is compatible with both jQuery and Zepto.js. Oh, and the licensing terms are simple: [just do what you want](http://refreshless.com/nouislider/terms-of-use).

Documentation
-------

An extensive documentation, including **examples**, **options** and **configuration details**, is available here: [noUiSlider documentation](http://refreshless.com/nouislider/).

Changes
-------

**Changelog for version 4.3.0:**
+ Added support for inverted (right-to-left and bottom-to-top) sliders.
+ Added a new `block` callback.
+ Added new options and features to `serialization`:  
  + Added option to serialize to a `function`.
  + Added option to serialize to any jQuery/Zepto element using any function.
  + Serialization fields are now filling upon initialization.
  + All settings within serialization are now optional.
  + The `to` option now optionally accepts an array of items to serialize to.
+ Fixed implementation of the `margin` option.
+ Fixed certain browsers showing the text selection cursor on drag.
+ Fixed an issue where an unintended `mouseup` on a slider might cause a 'tap'.
+ Fixed compatibility with `$.noConflict()`.
+ Simplified handle stacking order. **Check your css when upgrading!** A minor change is required. See the chapter on [styling](http://refreshless.com/nouislider/slider-design-styles) for more information.
+ Re-licensed to [WTFPL](http://www.wtfpl.net/about/). This changes nothing but the license name. The text and terms are identical.
+ Settings for `margin` and `step` are now applied to `.val()` input and the `start` option.
+ Reduced redundant event firing to make performance on older devices snappier. Events will no longer keep firing endlessly when a handle has hit a limit.


Version numbering
------------------------------
Version numbering follows the 'Semantic versioning' style.  
You'll find an excellent documentation at [Semver.org](http://semver.org/).

Compression and Error checking
------------------------------
**CSS** ([CSSMinifier](http://cssminifier.com/))  
The stylesheet is trimmed of whitespace and comments to provide a `min` version.

**JS** ([Google Closure Compiler](http://closure-compiler.appspot.com/home))  
The plugin is compressed using the Google Closure compiler, using the 'simple' optimization option.

**Code** ([JsLint](http://jslint.com/))  
The plugin code is checked using JsLint, with the following options:
```
browser: true
devel: true
plusplus: true
unparam: true
white: true
continue: true
```

Known issues
------------
There are some minor issues remaining in noUiSlider. It is a priority to fix these issues, but they may be fixed by browser changes in the future.

+ Firefox and Safari on Windows will emulate mouse-events on touch screens, but prefer scrolling to dragging the slider.
