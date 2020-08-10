[Motivation for this note](https://www.youtube.com/watch?v=90gFFdzuZMw&t=149s)

# Strings Sucks
Strings are defined as an array of characters. The difference between a character array and a string is the string is terminated with a special character ‘\0’.
Hence there is no primitive data type of strings like in C++ or python .

# Initializing Strings
This is the most critical part and string's declaration will tell us how string will be treated in our program.
```
char *name = "Utkarsh" ; // string literal, stored as read only data.
char another_name[] = "Utkarsh" // character array intialized from string literal, copied to and stored on the stack.
char another_name2[] = { 'U' , 't' , 'r' , 's' , 'h', '\0'}; // Same as above.
```
Now, we have seen all possible ways of declaring and initialization of string now difference between them.
For string literal,
	```
	name = "Divit" ; // In this statement we are changing the address name was earlier pointing to.
	name[4] = "U" ; // This is wrong  as string literal is not modifiable if we try to modify them we will incouter segmentation fault.
	```
For character array,
    ```
    another_name[] = "Divit" // Not possible as another_name[0] or it's base address is pointing to 'U'
    strcpy(another_name,"Utkarsh Singh"); /* Partially possible as another_name[] on time of declaration had size of
    7 byte this can be made possible be allocating more storage ie declaring another_name[20] */
    another_name[4] = 'K' // It's perfect
    ```
