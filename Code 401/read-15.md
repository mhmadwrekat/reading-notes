# Trees

> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|Quiz|First Paragraph|
|Trees|Second Paragraph|
|Answers|Last Paragraph|

---
## Quiz

1. Some Type Of Trees ?
2. What is a **Leaf** ?
3. What is a  **Root** ?
4. Three methods for depth first traversal ?
5. What is a **Binary Search Trees** ?

---
***Traversals***

An important aspect of trees is how to traverse them. Traversing a tree allows us to search for a node, print out the contents of a tree, and much more! There are two categories of traversals when it comes to trees:

- Depth First
- Breadth First

***Depth First***

Depth first traversal is where we prioritize going through the depth (height) of the tree first. There are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root. Here are three methods for depth first traversal:

1. Pre-order: root >> left >> right
2. In-order: left >> root >> right
3. Post-order: left >> right >> root

***Binary Tree Vs K-ary Trees***

In all of our examples, we’ve been using a Binary Tree. Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).

---
**Node** - A Tree node is a component which may contain it’s own values, and references to other nodes .

**Root** - The root is the node at the beginning of the tree .

**K - A** - number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2 .

**Left** - A reference to one child node, in a binary tree .

**Right** - A reference to the other child node, in a binary tree .

**Edge** - The edge in a tree is the link between a parent and child node .

**Leaf** - A leaf is a node that does not have any children .

**Height** - The height of a tree is the number of edges from the root to the furthest leaf .

---
***K-ary Trees***

If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree. In this type of tree we use K to refer to the maximum number of children that each Node is able to have.

***Breadth First Traversal***

Traversing a K-ary tree requires a similar approach to the breadth first traversal. We are still pushing nodes into a queue, but we are now moving down a list of children of length k, instead of checking for the presence of a left and a right child.


***Binary Search Trees***

A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right

***Searching a BST***

Searching a BST can be done quickly, because all you do is compare the node you are searching for against the root of the tree or sub-tree. If the value is smaller, you only traverse the left side. If the value is larger, you only traverse the right side.



![Trees](https://lh3.googleusercontent.com/proxy/fOALsO92rUGYuyddLpWqTEm7KvucOv72VmYHxmWWlQySs2vd4r5_5axdXdn3HEWLfbBeyhrQoDVktEk14Gk3rFpjZCtEgAKC-jHGvC9WRkjRESXVzQ)

---
## Answers 

1. **Some Type Of Trees ?**
   - Binary Trees .
   - Binary Search Trees .
   - K-ary Trees .


2. What is a **Leaf** ?

    **Leaf** - A leaf is a node that does not have any children3.


3. What is a  **Root** ?
 
    **Root** - The root is the node at the beginning of the tree .


4. Three methods for depth first traversal ?

   1. Pre-order: root >> left >> right
   2. In-order: left >> root >> right
   3. Post-order: left >> right >> root

5. What is a **Binary Search Trees** ?

    A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right


---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>