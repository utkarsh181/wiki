This note will only act as a source for useful links related to JS basics.

# Intro To Javascript
[MDN Docs For JS definition](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript)

JavaScript is a scripting language that enables you to create dynamically updating content, control multimedia, animate images, and pretty much everything else. (Okay, not everything, but it is amazing what you can achieve with a few lines of JavaScript code.)

Pro Tip : Everything thing in JS is a **object** and all types except object type are **immutable**.

# Add JS to your HTML
In your .html file, enter this code on a new line, just before the closing </body> tag:
```
<script src="main.js"></script>
```
If the JavaScript loads first and it is supposed to affect the HTML that hasn't loaded yet, there could be problems. Placing JavaScript near the bottom of an HTML page is one way to accommodate this dependency.

# Variables
[MDN Docs on JS Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)

Variables are containers that store values. You start by declaring a variable with the var (less recommended, dive deeper for the explanation) or the let keyword, followed by the name you give to the variable:

```
let myVariable; // This is camel case style on naming variable.
```

- [Semicolons in JS](https://news.codecademy.com/your-guide-to-semicolons-in-javascript/)
- [Naming Rules](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_Types#Variables)
- [Case Style For Variables](https://medium.com/better-programming/string-case-styles-camel-pascal-snake-and-kebab-case-981407998841)
- [Why to use let over var](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Variables#The_difference_between_var_and_let)
- [Data Types And Structure](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures) // **Just read this**
- [Why to use Camel Case In JavaScript ](https://stackoverflow.com/questions/33094418/why-use-camel-case-for-js-and-snake-case-for-your-db)

## null and undefined
[Stack Overflow Explanation](https://stackoverflow.com/questions/5076944/what-is-the-difference-between-null-and-undefined-in-javascript)

```
// typeof on undefined.
alert(typeof null); // returns object.
```
Quote from the book Professional JS For Web Developers (Wrox): "You may wonder why the typeof operator returns 'object' for a value that is null. This was actually an error in the original JavaScript implementation that was then copied in ECMAScript. Today, it is rationalized that null is considered a placeholder for an object, even though, technically, it is a primitive value."

# Comment
You can write comments in JavaScript just as you can in CSS:

```
// Comment without line break

/*
Everything in between is an comment.
*/
```

# Expression And Operators

[MDN Docs For Operators And Expression](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators)

[State Of Equality Operators](https://stackoverflow.com/questions/359494/which-equals-operator-vs-should-be-used-in-javascript-comparisons)

# Strings
```
let sampleStr = "Alan said, \"Peter is learning JavaScript\"."; // '\' works like escape sequence.
```
Some important escape sequence :
- \' - single quote
- \" - double quote
- \\ - backslash
- \n - newline
- \r - carriage return
- \t - tab
- \b - word boundary
- \f - form feed

Strings in js is immutable.

```
let foo = "Utkarsh";

foo[2] = 'k' ; // This is not throw any error but foo will be unchanged.

let foo = ['u', 't', 'k', 'a',  'r' , 's', 'h'];

foo[2] = 'c' ; // This is not same as above but will give us u,t,c,a,r,s,h but this differ from "utcarsh".
```
Difference between string and boolean.

```
let bool = true ; let string = "true" ; // true is a boolean data type whereas "true" is a string.
```

# Conditionals

- [if..else](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else)
- [switch](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch)

# Truth and False value

False Value -
- false
- 0
- "" // Empty String
- null
- undefined
- NaN // Not A Number

Everything else in truth.

# Iteration

[MDN Docs on Iteration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)

# Function

[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function)

# Events

Real interactivity on a website requires events handlers. These are code structures that listen for activity in the browser, and run code in response. The most obvious example is handling the click event, which is fired by the browser when you click on something with your mouse.

Ex -
```
document.querySelector('html').onclick = function() {
    alert('Ouch! Stop poking me!');
}
```
