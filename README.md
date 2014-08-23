# Sass Direction Controller

An approach to write a css code for once and create tow version of it RTL or LTR just with change one variable value

-----------------------

### Installation

* `_direction-controller.scss`:  It's main file to handle directions and have to import after $text-direction variable.

### Function/Mixin & Variabels

## Variable:

* `$text-direction`: Main variable to choose direction. Default value is ltr
* `$start`: If $text-direction value equal ltr, $star value is 'left'
* `$edn`: If $text-direction value equal ltr, $end value is 'right'


## Functions:

* `dir-check($a, $b)`: This function check if direction equal ltr return first parametr, else return secound parameter
* `dir-values($values)`: Reorder right and left positions in padding/margin values list
* `br-values($values)`: Reorder right and left positions in border-radius values list


## Mixin:

* `if-ltr() { @content }`: This Mixin check your direction and if your direction was ltr load content of this mixin.
* `if-rtl() { @content }`: This Mixin check your direction and if your direction was rtl load content of this mixin.

# More Info

Read details on this article(Persian): http://parhum.net/blog/ui/sass-direction-controller/