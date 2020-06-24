# INTRODUCTION TO HEAPS

[Wiki For Heaps](https://en.wikipedia.org/wiki/Heap_%28data_structure%29)
In computer science, a heap is a specialized tree-based data structure which is essentially an almost complete[1] tree that satisfies the heap property: in a max heap, for any given node C, if P is a parent node of C, then the key (the value) of P is greater than or equal to the key of C. In a min heap, the key of P is less than or equal to the key of C.[2] The node at the "top" of the heap (with no parents) is called the root node.

The heap is one maximally efficient implementation of an abstract data type called a priority queue, and in fact, priority queues are often referred to as "heaps", regardless of how they may be implemented. In a heap, the highest (or lowest) priority element is always stored at the root. However, a heap is not a sorted structure; it can be regarded as being partially ordered. A heap is a useful data structure when it is necessary to repeatedly remove the object with the highest (or lowest) priority.

One common confusion with binary heap are sometimes they are often compared with BST(Binary Search Tree) but they are are tree based and not search-tree based data structure.

# OPERATION ON BINARY HEAPS

Generally binary heap are implemented using arrays. Since C follow 0-based indexing in arrays we will implement binary heap in this format also.
[This post](https://stackoverflow.com/questions/22900388/why-in-a-heap-implemented-by-array-the-index-0-is-left-unused) explains how elements are arranged in binary heap and how their parent and children can be identified.

## INSERTION AND DELETION IN BINARY HEAPS

[Geek For Geek For operation on heaps](https://www.geeksforgeeks.org/insertion-and-deletion-in-heaps/)
1. Time complexity for Insertion : O(log n)
Where (log n) represents height of tree required to rearrange after insertion and n represents number of nodes to rearrange , hence for inserting n elements in binary heaps time complexity is O(n * log n).
2. Time complexity for Deletion : //TODO
