# Lecture 2 (1/8/25)

## Things I'm confused about 
### how to calculate big O 

## After class TODO
- 

## Things I'm confused about 

___
## Notes
### Trees
Terms
- Node
- Branch (edge)
- Parent, child, siblings
- Ancestor, descendant
- Height (many definitions): maximal level of any node
  -  If root as level 0, height of this tree: 3
  -  If root as level 1, height of this tree: 4
- Can be defined using a recursive definition.
  – T is a tree if:
    - T is empty, or
    - T has a node and zero or more non-empty subtrees (each of which is also a tree.)
### Binary tree
- At most 2 children <br/>

struct BinaryTreeNode {<br/>
  Object *item;<br/>
  BinaryTreeNode *leftChild;<br/>
  BinaryTreeNode *rightChild;<br/>
};<br/>

- Many uses
  - Expression tree
  - Huffman coding algorithm
  - Binary search tree
  - etc.
- Will include a binary tree implementation in assignment 2


- **Full binary** tree has no nodes with one child; they all have
zero or two.
- **Perfect binary tree**: full binary tree where all of the leaves
are at the same level
- **Complete binary tree** has every level, except possibly the
deepest, is completely filled. The nodes in the last level
are as far left as possible
- **Balanced binary tree**: where the left and right subtrees of
any node have height difference by at most 1 (ignore leaves)
<img width="341" alt="Screenshot 2025-01-08 at 18 48 37" src="https://github.com/user-attachments/assets/b343dd28-f778-4bff-8c8f-f87962a4b135" />

<img width="923" alt="Screenshot 2025-01-08 at 18 53 35" src="https://github.com/user-attachments/assets/8ee6cb00-627f-45c2-b162-5aaf2b899653" />
- # of nodes = n
- min level = log n
- max level = n


