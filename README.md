# totogram

A Totogram is a puzzle played on a board that has a graph structure, with edges connecting some pairs
of vertices. The edges of the graph form a rooted tree with a particular structure: the root has exactly
three children, every other non-leaf node has exactly two children, and the leaves are all at the same
depth k in the tree. This graph has the property that every vertex has exactly 1 or 3 neighbors.
To play the Totogram, the player arranges a set of N tiles numbered from 1 to N, where N is the number of vertices in the graph (which, in turn,is a function of k), on the vertices of the board. Their score is equal to the maximum absolute value of the difference between any pair of adjacent vertices, and the goal is to find an arrangement that makes the score as low as possible.
totogram.py is an implementation of above puzzle returning the low scores possible.
I have implemented a tree with three nodes in level two and each having two children at every other level.I used reursion for this implementation.
