Kickass LESS Syntax
===================
#### a syntax mode for [Coda](http://panic.com/coda) & [SubEthaEdit](http://www.subethaedit.net/) ####


Installation
------------
1. Extract to `~/Library/Application Support/Coda/Modes/LESS.mode`
2. Restart your code editor


Change Log
----------

###2.2###

* Added math functions (`round()`, `ceil()`, `floor()`, and `percentage()`)
* Added new color functions (`mix()`, `color()`, `argb()`)
* Added detection for ARGB colors, e.g. #80FF00FF (violet with a 50% alpha)
* Made color function highlighting more specific (now requires them to be followed by a paren)
* Fixed class selectors being interpreted as mix-ins if followed by a pseudo-selector (namely, a colon)

Example
----------
![screenshot of example code](https://github.com/elstgav/LESS.mode/raw/master/screenshot.png)

*Example using [Solarized](http://ethanschoonover.com/solarized) Colors*

Features
--------
Kickass LESS Syntax detects:

* CSS Rules: `@import`, `@media`, `!important`

* Selectors
	* CSS Selectors: `#id`, `.class`
	* HTML Elements: `body`, `div`, etc.
	* Pseudo Selectors: `:hover`, `::before`, `:nth-child()`, etc.
	* Operators: `&`,`*`, `>`, `+`, `~`

* Variables
	* Standard: `@var` 
	* Definitions: `@var: 2;`
	* Interpolated: `"@{var}"`

* Mixins: `.mixin();`, `.mixin;`

* Color Functions: `lighten()`, `darken()`, `saturate()`, `desaturate()`, `fade()`, `fadein()`, `fadeout()`, `spin()`, `mix()`, `argb()`

* Math Functions: `round()`, `ceil()`, `floor()`, `percentage()`

* JavaScript: `` `"@{str}".toUpperCase();` ``

Notes for contributors
------------------------------------

This syntax mode is based on the [SubEthaEdit Mode File Format](http://www.codingmonkeys.de/subethaedit/mode.html). Read the [documentation](http://www.codingmonkeys.de/subethaedit/mode.html) to learn about the structure and syntax. The meat of the syntax mode lives in `/Contents/Resources/SyntaxDefinition.xml`, so go there to see how the sausage is made.

###Regular Expressions###
*	Flavor: Ruby
*	Escape: \
*	Multiline, With Capture Groups


Credits
-------

Original work by [Jose Prado](http://pradador.com/).  This copy forked by [Gavin Elster](https://github.com/elstgav) from [Jake Strawn's version](https://github.com/himerus/LESS.mode).