# INHERITENCE
[MDN Docs For Inheritence](https://developer.mozilla.org/en-US/docs/Web/CSS/inheritance)
In CSS, inheritance controls what happens when no value is specified for a property on an element.

# INHERITED PROPERTIES
When no value for an inherited property has been specified on an element, the element gets the computed value of that property on its parent element.The computed value is nothig but specficity of that element.

Example:

```
p {
	color: green;}
```

```
<p>This paragraph has <em>emphasized text</em> in it.</p>
```
The words "emphasized text" will appear green, since the em element has inherited the value of the color property from the p element.


# SPECIFICITY
[MDN Doc For Specificity](https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity)
Specificity is the means by which browsers decide which CSS property values are the most relevant to an element and, therefore, will be applied.

## ORDER OF SPECIFICITY

As we go down specficity increases.

1. Type selectors (e.g., h1) and pseudo-elements (e.g., ::before).
2. Class selectors (e.g., .example), attributes selectors (e.g., [type="radio"]) and pseudo-classes (e.g., :hover).
3. ID selectors (e.g., #example).
