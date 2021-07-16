# Read: Trees



## Define the following terms:

- Node : A Tree node is a component which may contain it’s own values, and references to other nodes.
<br/>

- Root : The root is the node at the beginning of the tree.
<br/>


- K : A number that specifies the maximum number of children any node may have in a k-ary tree. 
<br/>

- Left : A reference to one child node, in a binary tree `k = 2`.
<br/>

- Right : A reference to the other child node, in a binary tree.
<br/>

- Edge : The edge in a tree is the link between a parent and child node.
<br/>

- Leaf : A leaf is a node that does not have any children.
<br/>


- Height : The height of a tree is the number of edges from the root to the furthest leaf.

<br/>
<br/>
<br/>

# Tree configuration:
![](../images/sampleT.png)

<br/>
<br/>
<br/>

## How to traverse through a tree?
- There are two methods for traversing trees:
   1. Depth First
   2. Breadth First

<br/>
<br/>
<br/>

## What is depth first traversal ?
- It is where we prioritize going through the depth (height) of the tree first.
<br/>


### Here are three methods for depth first traversal:
1. Pre-order : `root >> left >> right`
2. In-order : `left >> root >> right`
3. Post-order : `left >> right >> root`

<br/>



> Note: The most common way to traverse through a tree is to use recursion.


<br/>



## what is Breadth First traversal?
-It iterates through the tree by going through each level of the tree node-by-node.

<br/>
<br/>

## Binary Tree Vs K-ary Trees
1. Binary Trees restrict the number of children to two (hence left or right).
2. If Nodes are able have more than 2 child nodes, we call the tree that contains them a **K-ary Tree**.

<br/>

> We use K to refer to the maximum number of children that each Node is able to have.

<br/>
<br/>

## The big O notation:

- The Big O time complexity of a Binary Search Tree’s insertion and search operations is O(h), or O(height).
<br/>

- In a balanced (or “perfect”) tree, the height of the tree is log(n).
<br/>


- The Big O space complexity of a BST search would be O(1). 

<br/>
<br/>
<br/>

# References:

1. [Read: Trees](Read: Trees)
