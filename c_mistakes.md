# Cast the result of malloc
[Link to stackoverflow](https://stackoverflow.com/questions/605845/do-i-cast-the-result-of-malloc)
1. void* is automatically and safely promoted to any other pointer
2. repeating things are bad

# `sizeof` is a function
[Link to stackoverflow](https://stackoverflow.com/questions/1393582/why-is-sizeof-considered-an-operator)
1. The parentheses are unnecessary
2. The operand of sizeof can be parenthesized
3. `int array_name[sizeof (int)] = {0}` does not return error which is it can be used as compile time constant, which is possible if it's is a operator.

```
int a;
printf("%li",sizeof a) // returns 4
printf("%li",sizeof (int)) // returns 4, but here we are type-casting are int and not giving sizeof int as parameter
```
