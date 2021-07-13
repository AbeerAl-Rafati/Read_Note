# Trees 

* A tree is a nonlinear data structure, compared to arrays, linked lists, stacks and queues which are linear data structures. A tree can be empty with no nodes or a tree is a structure consisting of one node called the root and zero or one or more subtrees.   



`Node` - A Tree node is a component which may contain it’s own values, and references to other nodes  
`Root` - The root is the node at the beginning of the tree  
`K` - A number that specifies the maximum number of children any node may have in a k-ary tree.
`Left` - A reference to one child node, in a binary tree   
`Right` - A reference to the other child node, in a binary tree   
`Edge` - The edge in a tree is the link between a parent and child node   
`Leaf` - A leaf is a node that does not have any children   
`Height` - The height of a tree is the number of edges from the root to the furthest leaf   


- Depth-first search (DFS)  
 is an algorithm for traversing or searching tree or graph data structures.   

- depth first traversal methods   
  
> Pre-order: `root >> left >> right`   
In-order: `left >> root >> right`   
Post-order: `left >> right >> root`   


- Breadth-first search   
 is an algorithm for searching a tree data structure for a node that satisfies a given property.    



 - Binary Tree Vs K-ary Trees   

`K-ary tree` is a rooted tree, where each node can hold at most k number of children.   

`A binary tree` is a rooted tree that is also an ordered tree (a.k.a. plane tree) in which every node has at most two children. 