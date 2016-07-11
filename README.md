#Totogram  

A Totogram is a puzzle played on a board that has a graph structure, with edges connecting some pairs
of vertices.The edges of the graph form a rooted tree with a particular structure: the root has exactly three children, every other non-leaf node has exactly two children, and the leaves are all at the same depth k in the tree. This graph has the property that every vertex has exactly 1 or 3 neighbors. 

##Game Strategy
To play the Totogram, the player arranges a set of N tiles numbered from 1 to N, where N is the number of vertices in the graph (which, in turn, is a function of k), on the vertices of the board. Their score is equal to the maximum absolute value of the difference between any pair of adjacent vertices, and the goal is to find an arrangement that makes the score as low as possible.

##Sample Totogram

![alt tag](https://github.com/Nethracs/totogram/blob/master/totogram.png)

##Algorithm
 Step1:Find the total number of nodes for the given height, function num_nodes() is implemented to compute this.  
 Step2:call on function medians() to compute median and it creates a list which as all the medians.  
 Step3:function leveltree() is called to build a balanced binary tree with an exception at level two which has three nodes  
 Step4:diff() is called to find the maximum difference in built tree.  
 Step5:loop is constructed which call the function optimize() to reorders the tree to reduce the maximum difference found so far.  
 Step6:loop terminates if no more optimization could be made with the tree constructed.  
 
##Steps to run the code
 python totogram.py k
 
 Where k is depth of the tree







