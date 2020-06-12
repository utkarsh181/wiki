# BOX MODEL IN CSS
[MDN Docs For Box Model](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model)
When laying out a document, the browser's rendering engine represents each element as a rectangular box according to the standard CSS basic box model. CSS determines the size, position, and properties (color, background, border size, etc.) of these boxes.

# CONTENT AREA
The content area, bounded by the content edge, contains the "real" content of the element, such as text, an image, or a video player.

Example of operation on content area:

```
h1{
	width: 20px;
	hight: 20px;
}
```
Here hight and width of the header element will change to 20px each.

## USEFUL TAGS FOR CONTENT AREA

1. To make text uppercase : `text-transform: uppercase`
2. To align text : `text-align: center`
3. To make spacing between letters: `letters-spacing: 3px`
4. To make spacing between words: `word-spacing: 5px`
5. To make text float( ie to break flow of document ): `float: left`

# BORDER AREA
The border area, bounded by the border edge, extends the padding area to include the element's borders. Its dimensions are the border-box width and the border-box height.

```
h1{
	border: 2px solid blue;
}
```

This will make border of 2px of solid type with blue color.

## USEFUL TAGS FOR BORDER AREA

1. To make border on a given side: `border-left` , `border-right` , `border-bottom` etc.
2. To make border adjust to page size: `border: 10%`

# PADDING AREA
The padding area, bounded by the padding edge, extends the content area to include the element's padding or space between border an content.

```
h1{
	padding-left: 20px ;
	padding-right: 30px ;
}
```
This will introduce 20px space between content and border on right and left to make equal amount of padding in all direction we can use `padding:`.

Most of the properties working on border area will work on padding area.

# MARGIN AREA

Margin Area is the area outside the border used to separate the element from its neighbors.

```
h1{
	margin: 100px;
}
```
This will introduce margin of area 100px outside of border.

Most of the properties working on border area will work on margin area.
