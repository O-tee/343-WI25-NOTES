# Chapter 15
Chapter 15 of the source Frank M. Carrano, Timothy Henry - Data abstraction & problem solving with C++ _ walls and mirrors (2017) discusses trees, a data structure that represents relationships.  Trees are used for representing relationships, such as the relationship between the calls of a recursive algorithm. <br/>

There are different types of trees, such as:
- **General trees**: They consist of a single root node and sets of general trees called subtrees.
- **N-ary trees**:  They are a set of nodes that is either empty or partitioned into a root node and up to n subtrees. Each node can have no more than n children.
- **Binary trees**: They consist of nodes with up to two children, referred to as the left child and the right child. The chapter discusses the properties and terminology associated with binary trees, including the root, parent, child, sibling, ancestor, descendant, leaf, level, and height.
- **Binary search trees**:  They are a specialized type of binary tree where the data in the left subtree of a node is always less than the data in the node, and the data in the right subtree is always greater than the data in the node. <br/>

The chapter discusses operations on binary search trees, including searching, adding data, and removing data, as well as traversal methods. The chapter provides examples of using trees, including building binary trees and binary search trees. It also discusses the efficiency of binary search tree operations. The chapter explains that the height of a binary search tree affects the efficiency of the retrieval, addition, and removal operations. Operations on a balanced binary search tree that has a height close to log2n are more efficient. Chapter 19 will discuss variations of the basic binary search tree that are guaranteed always to remain balanced.

# Chapter 16
Chapter 16 of Frank M. Carrano, Timothy Henry - Data abstraction & problem solving with C++ _ walls and mirrors (2017), building on the concepts introduced in Chapter 15, focuses on implementing the binary tree and binary search tree ADTs using C++.

## Implementation of Binary Trees
- Nodes:  Each node in a binary tree is represented as an object containing data and pointers to its children. There are two main implementation approaches:
  - Array-based Implementation: Nodes are stored in an array, and their positions in the array determine the parent-child relationships. This implementation is efficient for complete binary trees, where all levels are full except possibly the last, which is filled from left to right.
  - Link-based Implementation:  Nodes are linked together using pointers. Each node contains two pointers, one to its left child and one to its right child, in addition to its data. This implementation is more common and flexible, suitable for binary trees of various shapes.
- Traversals: The chapter explains and provides pseudocode for the three standard traversal methods for binary trees:
  - Preorder Traversal: Visit the node, traverse the left subtree, traverse the right subtree.
  - Inorder Traversal: Traverse the left subtree, visit the node, traverse the right subtree.
  - Postorder Traversal: Traverse the left subtree, traverse the right subtree, visit the node.
- Recursive vs. Non-recursive Implementations:  The chapter presents both recursive and non-recursive implementations for traversal methods. Non-recursive implementations use an explicit stack to mimic the implicit stack used in recursive calls.

## Implementation of Binary Search Trees
- Operations: The chapter provides algorithms and pseudocode for the key operations of the ADT binary search tree, assuming a link-based implementation:
  - Adding a new entry: The algorithm adds the new entry in the same position where the search algorithm would look for it, maintaining the sorted order.
  - Removing an entry: The algorithm handles different cases depending on the number of children the node to be removed has.

## Saving and Restoring Binary Search Trees
- Saving:  The chapter discusses two algorithms for saving a binary search tree to a file for later restoration:
  - Saving the tree in its original shape: This algorithm saves the tree using a preorder traversal.
  - Saving the tree in a balanced shape: This algorithm builds a balanced binary search tree from the sorted data.

## General Trees
- The chapter briefly discusses general trees and how they can be implemented as binary trees.

Chapter 16 emphasizes that the implementation of a binary tree affects the efficiency of its operations. Understanding these implementations is crucial for efficiently managing data using trees.
