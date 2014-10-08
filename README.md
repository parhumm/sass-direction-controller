# Sass Direction Controller

An approach to write a css code for once and create tow version of it RTL or LTR just with change one variable value

-----------------------

# Installation

* `_direction-controller.scss`:  It's main file to handle directions and have to import after $text-direction variable.

# Document

### Direction Controller Settings

* `$text-direction`: Main variable to change css output for RTL / LTR websites. Default value is **ltr**
* Direction Controller base is for LTR languages. If you want change default coding Sass structure for RTL languages, change default value of these variables:
	* `$default-float`: Default value is **left**
	* `$opposite-direction`: Default value is **right**

### Useful Variable

* `$text-direction`: Main variable to choose direction. Default value is ltr
* `$start`: If **$text-direction** value equal **ltr**, `$start` value is **left**
* `$end`: If **$text-direction** value equal **ltr**, `$end` value is **right**


### Useful Functions

* `dir-check($a, $b)`: This function check if direction equal ltr return first parametr, else return secound parameter
* `dir-values($values)`: Reorder right and left positions in padding/margin values list
* `br-values($values)`: Reorder right and left positions in border-radius values list

### Useful Mixins

* `if-ltr() { @content }`: This Mixin check your direction and if your direction was ltr load content of this mixin.
* `if-rtl() { @content }`: This Mixin check your direction and if your direction was rtl load content of this mixin.

# More Info

Read details on this article(Persian): http://parhum.net/blog/ui/sass-direction-controller/

# Changelog

### 1.0.0
* Add `$default-float` & `$opposite-direction` variables to can change base Sass structure for LTR / RTL. Default structure is for `LTR` languages

### 0.2.0
* Change `$left` & `$right` variable names to `$start` & `$end`

### 0.1.0
* initial release