# SETTING FONTS-FAMILY IN CSS
[MDN Docs For Font-Family](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family)
The font-family CSS property specifies a prioritized list of one or more font family names
 and/or generic family names for the selected element.

Example:
```
h1{
	font: Arial;
}
```
This will make h1 of Arial font-family.

# SETTING FONTS SIZE IN CSS
[MDN Docs For Font Size](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size)
[More About Size in Css](https://www.w3schools.com/CSSref/css_units.asp)
The font-size CSS property sets the size of the font.

## USING PIXEL METHOD
This is a recommend way when we need pixel accuracy.But is browser and os dependent.
Example:
```
h1{
	font-size:20px ;
}
```
This will make h1 of size 20px.

## USING EM METHOD
Another way of setting the font size is with em values. The size of an em value is dynamic. When defining the font-size property, an em is equal to the font size of the element on which the em is used. Em are very important as they are default unit of measurement in bootstrap.

Example ( Standard Trick For Web Development ):
```
body{
	font-size : 10px;
}

h1{
	font-size: 5em;
}

p{
	font-size: 3em;
}

```
# SETTING FONTS WEIGHT IN CSS
The font-weight CSS property sets the weight (or boldness) of the font. The weights available depend on the font-family you are using.

Example:
```
h1{
	font-weight: 600 ;
}

```
font-weight ranges from 100-800 for every multiple of 100.

1.400 = Normal
2.>400 = Lighter
3.<400 = Bolder

# SETTING LINE HEIGHT IN CSS
As name suggest line height is used to determine line height of a font. By default line height depends on font size and font used.


Example:

```
h1{
	line-height: 1.5;
}
```
This will multiply present line height to 1.5 and hence increasing it by 50%.

# SETTING LINE ALIGNMENT IN CSS

Example:

```
h1{
	text-align: center;
}
```
This will align header 1 to center.

# SETTING TEXT DECORATION IN CSS

Example:

```
h1{
	text-decoratoion: underline;
}

```
# SETTING TEXT SHADOW IN CSS
The text-shadow CSS property adds shadows to text. It accepts a comma-separated list of shadows to be applied to the text and any of its decorations. Each shadow is described by some combination of X and Y offsets from the element, blur radius, and color.

Example:

```
text-shadow: 1px 1px 2px pink;
```
This will introduce a text shadow of 1px in x and y coordinate of 2px radius of pink color.
