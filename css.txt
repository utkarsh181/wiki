# INTRODUCTION TO CSS
[MDN Docs For CSS Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics)
Like HTML, CSS is not really a programming language. It is not a markup language either — it is a style sheet language. This means that it lets you apply styles selectively to elements in HTML documents.

# HOW TO LINK CSS TO HTML:

## METHOD 1
Using css code inside html file.

```
<head>

</head>
```
This method can be used during debugging or writing small code but not a recommended way.

## METHOD 2

Using external css file and link it to html file this statement should be inside a `<head>` element in css.

```
<link rel="stylesheet" type="text/css" href="path_to_file.css">

```
If file is in same directory as of html file than only file name should be specified.

# HOW TO COMMENT IN CSS FILE
Example:

```
/* p{
	background: url(image);
}*/
```

# GENERAL RULE FOR CSS
```
selector{
	property: value;
	anotherProperty: value;
}
```
Example:

![css-declaration-small.png](resources/36acea014dd8433aa29f9a9faf91e051.png)

## SELECTOR
The HTML element name at the start of the rule set. It selects the element(s) to be styled (in this case, `<p>` elements). To style a different element, just change the selector.

## PROPERTIES
Ways in which you can style a given HTML element. (In this case, color is a property of the `<p>` elements.) In CSS, you choose which properties you want to affect in your rule.

## PROPERTY VALUE
To the right of the property, after the colon, we have the property value, which chooses one out of many possible appearances for a given property (there are many color values besides red).

Note the other important parts of the syntax:

1. Each rule set (apart from the selector) must be wrapped in curly braces ({}).
2. Within each declaration, you must use a colon (:) to separate the property from its values.
3. Within each rule set, you must use a semicolon (;) to separate each declaration from the next one.

# COLOR IN CSS

## USING NAME

Example :

```
h1{
	color : purple ;
}
```

## USING HEXADECIMAL
#+ String Of 6 heaxadecimal number from 0-F

Example:
```
h1{
	color: #OOOOOO;
}
```
## USING RGB()
3 channels:Red,Green,and Blue. Each ranges from 0-225

```
h1{
	color: rgb(12,12,13);
}
```
## USING RGBA()
Just like RGB(),but with an alpha(transperancy) channel. Ranges from 0.0-1.0 .

```
h1{
	color: rgba(12,12,13,.2);
}
```

# COLOR AND BACKGROUND
backgroud is used to set background color and color is used for text color.

```
body{
	background: #981111;
}

p{
	color: #533322;
}
```
To set a image as a background image.
```
backgroud : url(any link for backgroud inmage)

```
To stretch a image to cover full screen.

```
background-repeat: no-repeat;
background-size: cover ;
```
To make borders in CSS :
[MDN Docs For Border](https://developer.mozilla.org/en-US/docs/Web/CSS/border)

Border takes 3 value border-width , border-style and border-color.


```
border : 5px solid #111111 ;

```

# TYPES OF SELECTOR

## ELEMENT SELECTOR

This type of selector will select all element with the given name , which hadicap us to choose only one kind of style for that element.

```
<ul>
<li>First</li>
<li>Second></li>
</ul>
```
Example:
```
li{
	color: red;
}
```
This will make all elements in list as red.

## ID SELECTOR

Selects a element with a given ID. Only one unique ID is allowed in a page which means we cannot have 2 elements with same id.


```
<ul>
<li id="special">First</li>
<li>Second></li>
</ul>
```

```
#special{
	color: red;
}
```
This will only make First red.

## CLASS SELECTOR

Works like id but can be used multiple time in a page.
```
<ul>
<li class="special">First</li>
<li class="special">Second></li>
</ul>
```

```
.special{
	color: red;
}
```
Will make both First and Second red.


## OTHERS

### STAR SELECTOR

Just like * in unix-based os command line star(*) selects all the element in a page.

```
<ul>
<li class="special">First</li>
<li class="special">Second></li>
</ul>
```

```
*{
	color: red ;
}
```

### DECENDANT SELECTOR

This selector is used to select decendent of a given
selector.

```
<ul>
<li class="special">First</li>
<li class="special">Second></li>
</ul>
```

```
ul li{
	color: red ;
}
```
This will select all the li which are included inside ul tag.

### ADJACENT SELECTOR

This selector selects the adjacent selector at the same level.

```
<ul>
	<li>Apples</li>
	<li>Oranges</li>
	<li>Bananas</li>
</ul>

<h4>Popular Sites</h4>

<ul>
	<li>Carrots</li>
	<li>Peas</li>
	<li>Asparagus</li>
</ul>
```

```
h4 + ul {
	color: ref ;
}
```

This will select ul tag adjacent to h4 .

### ATTRIBUTE SELECTOR

This selector selects a checks for given attribute in an element , and thus helping us to style according to  attribute.

```
<ul>
	<li><a href="https://www.utkarsh.com">Utkarsh</a></li>
	<li><a href="https://www.singh.com">Singh</a></li>
</ul>
```
```
a[href="https://www.utkarsh.com"]{
	color : gold;
}
```
This will make Utkarsh gold.

### N'TH OF TYPE

This selector helps us to select nth element inside an element.

```
<ul>
	<li><a href="https://www.utkarsh.com">Utkarsh</a></li>
	<li><a href="https://www.singh.com">Singh</a></li>
</ul>

```

```
li:nth-of-type(1){
	color: blue ;
}
```
This will select firs li.
