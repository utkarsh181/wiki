# Objects

[MDN Docs on Objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)

# Accessing Objects

- Dot Notation
	```
	var myObj = {
	  prop1: "val1",
	  prop2: "val2"
	};
	var prop1val = myObj.prop1; // val1
	var prop2val = myObj.prop2; // val2
	```
- Bracket Notation

	If the property of the object you are trying to access has a space in its name, you will need to use bracket notation.
	```
	var myObj = {
	  "Space Name": "Kirk",
	  "More Space": "Spock",
	  "NoSpace": "USS Enterprise"
	};
	myObj["Space Name"]; // Kirk
	myObj['More Space']; // Spock
	myObj["NoSpace"];    // USS Enterprise
	```
	Bracket Notation is also useful when we use variables to access object difference is then we don't use `""` around variables name.

# Some Useful method

- .hasOwnProperty(propName)
	We can use the .hasOwnProperty(propname) method of objects to determine if that object has the given property name. .hasOwnProperty() returns true or false if the property is found or not.
