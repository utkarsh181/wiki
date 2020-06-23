# Arrays
[MDN Docs on array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

The JavaScript Array class is a global object that is used in the construction of arrays; which are high-level, list-like objects.Neither the length of a JavaScript array nor the types of its elements are fixed. Since an array's length can change at any time, and data can be stored at non-contiguous locations in the array, JavaScript arrays are not guaranteed to be dense; this depends on how the programmer chooses to use them. In general, these are convenient characteristics; but if these features are not desirable for your particular use, you might consider using typed arrays.

# 1-D Array
```
var array = ["Utkarsh" , 19 , true ] // Yes in js it is possible to create array with diffrent primitive data types
```
# Nested Array
```
var myArray = [["Bulls",23],["White Sox",45]];
```

Just like C/C++, js also uses 0 based indexing to access element in array. Some more obvious things first.

```
var myArray = [["Bulls",23],["White Sox",45]];

var myVar = myArray[0] // This returns array ["Bulls",23]

var myVar = myArray[0][1] // This returns integer 23

var myVar = myArray[0][2] // This returns undefined
```

JavaScript properties that begin with a digit cannot be referenced with dot notation and must be accessed using bracket notation.

```
let years = [1950, 1960, 1970, 1980, 1990, 2000, 2010]

console.log(years.0)   // a syntax error

console.log(years[0])
```

# Common operations
- arrayName.push(item) - Append array
- arrayName.pop() - Delete last element of array
- arrayName.shift() - Delete first element of array
- arrayName.unshift(item) - Add from front to array
