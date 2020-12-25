# INTRODUCTION TO HASH TABLE
[Geek For Geek link for Hash](https://www.geeksforgeeks.org/hashing-data-structure/)
Hash table is a data structure in which key are mapped to array position by a hash function.

# COMPONENTS OF HASH TABLE
1. Hash Function
2. Collision Resolution Method

# HASH FUNCTION
[Wiki For Hash Function](https://en.m.wikipedia.org/wiki/Hash_function)

A hash function is a mathematical formula which , when applied to a key , produce an interger which can be used as an index for the keys in the hash table

## PROPERTIES OF A GOOD HASH FUNCTION

1. Low Cost - The cost of executing a hash function must be small , so that using the hasing technique becomes prefreable over other apporaches.
2. Determinism - A hash procedure must generate same hash value for a given input value which means function should genrate same output during insertion and retrival process.
3. Uniformity - A good hash function must map the keys as evenly as possible over its output range. This uniformity is measured by loading factor ,that is, the proportion of the slots in the array that are used.

$$
 \gamma = Number of elements / size of hash , \gamma = LoadingFactor
$$

If

$$
 \gamma = 0.5
$$

then we say we have choosen a good hash.



# TYPES OF COLLISION RESOLUTION METHOD
We will be discussing only the methods which follows [open addressing ](https://en.wikipedia.org/wiki/Open_addressing).

## CHAINING
Eg :
Hash Function used:
$$
 h(x) = element \mod n
$$

In chaining , each location in a hash table store a pointer to a linked list that contains all the key value that were hashed to that location.
$$
AvgSuccesfullSearch = 1+\gamma/2
$$
$$
AvgUnsuccesfullSearch = 1+\gamma
$$

## LINEAR PROBING
[Wiki for linear probing](https://en.wikipedia.org/wiki/Linear_probing)
Hash FunctioN used:
$$
h(x) = ( h(x) + f(i) ) \mod n
$$
where
$$
f(i) = i , i=0,1,2...
$$
In linear probing , if h(x) is already filled then next position is found out by using f(i)
$$
AvgSuccesfullSearch = 1\div(\gamma)* ln(1\div(1-\gamma))
$$
$$
AvgUnsuccesfullSearch =ln(1\div(1-\gamma))
$$

## QUADRATIC PROBING
[Wiki for Quadratic probing](https://en.wikipedia.org/wiki/Quadratic_probing)
Eg :
Hash Function used:
$$
h(x) = ( h(x) + f(i) ) \mod n
$$
where
$$
f(i) = i^2 , i=0,1,2...
$$
Quadratic probing , causes less clustering than linear probing and hence resulting in better search time. But on the same time in the search of more space it leads to larger hash table which will lead to greater search time.

## DOUBLE HASHING

[Wiki for double hashing](https://en.wikipedia.org/wiki/Double_hashing)

Double Hashing works on idea that in case of collsion we can have a extra hash function which will help us
to look for index.
Eg :
Hash function used:

$$
h3(x) = ( h1(x) + i*h2(x) ) \mod n
$$
where
$$
f(i) = i , i=0,1,2...
$$

The main tradeoffs between these methods are that linear probing has the best cache performance but is most sensitive to clustering, while double hashing has poor cache performance but exhibits virtually no clustering; quadratic probing falls in-between in both areas. Double hashing can also require more computation than other forms of probing.

# TIPS FOR CHOSING HASH FUNCTION

When we are using any collison method another than chaining , then we should take size of the hash twice of number of elements we are inserting.Hence loading factor should be less than 0.5

It is preferred that size of hash should be a prime number because they have least number of factors which will lead to less number of collision

Diffrent Ideas For Hash Function:
1. Mod Function - Mod of the key is taken .
2. Midsquare - Middle digit of the key of choosen after performing squaring it.
3. Folding - This is completly condition dependent , various operation can be performed on key like adding all of it's digits and the choosing the most significant one.

ACSCII code can be used for special character and even char data type.
