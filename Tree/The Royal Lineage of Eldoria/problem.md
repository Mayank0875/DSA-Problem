## Title

The Royal Lineage of Eldoria

## Slug

the-royal-lineage-of-eldoria

## Difficulty

Medium

## Description

In the ancient kingdom of Eldoria, the royal family tree is recorded in a vast archive. The lineage is structured as a binary tree, where each member (node) has a unique royal ID. Disputes often arise regarding the inheritance of the throne, requiring the Royal Historian to determine the most recent common ancestor of two disputing heirs.

Given the royal family tree and two heirs, $p$ and $q$, your task is to find their **Lowest Common Ancestor (LCA)**. 

The lowest common ancestor is defined between two nodes $p$ and $q$ as the lowest node in the tree that has both $p$ and $q$ as descendants (where we allow **a node to be a descendant of itself**).

## Examples

### 1

#### Input

11
3 5 1 6 2 0 8 N N 7 4
5 1

#### Output

3

#### Explanation

The tree structure is:
      3
     / \
    5   1
   / \ / \
  6  2 0  8
    / \
   7   4
The LCA of heirs 5 and 1 is 3.
    
### 2

#### Input

11
3 5 1 6 2 0 8 N N 7 4
5 5

#### Output

5

#### Explanation

The LCA of heirs 5 and 4 is 5, because a node can be a descendant of itself according to the definition.
  

## Input Format  

- The first line contains an integer $n$, representing the number of nodes in the level-order representation of the tree.
- The second line contains $n$ space-separated strings representing the node values.

## Output Format  

- Return integer representing the value (royal ID) of the Lowest Common Ancestor node.
  

## Constraints  

- 1 ≤ n ≤ 1e4
- 1 ≤ node -> val ≤ 1e5
- All node -> val are unique.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search-tree

## Companies
infosys