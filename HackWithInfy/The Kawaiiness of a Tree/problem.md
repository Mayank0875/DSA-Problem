## Title

The Kawaiiness of a Tree

## Slug

the-kawaiiness-of-a-tree

## Difficulty

Medium

## Description

Behruzbek is studying the properties of trees. He has a tree with n vertices and has chosen an integer k.
He defines the cuteness of a tree rooted at a specific vertex r as follows:
Consider every possible set of k distinct vertices from the tree.
    1. For each set, find the Lowest Common Ancestor (LCA) of the vertices in that set, calculated with respect to the root r.
    2. Let S_r be the set of all unique vertices obtained as LCAs from these sets.
    3. The cuteness of the tree rooted at r is the size of S_r (denoted as |S_r|).

Behruzbek then defines the kawaiiness of the tree as the sum of the cuteness values for all possible roots r from 1 to n:
Kawaiiness = sum over r from 1 to n of |S_r|

Your task is to calculate the kawaiiness of the given tree.
Notes:
    1. A tree is a connected graph without cycles.
    2. The LCA of a set of nodes in a rooted tree is the deepest node that is an ancestor of all nodes in the set.

## Examples

### 1

#### Input

6 3
1 2
1 3
2 4
2 5
3 6

#### Output

17

#### Explanation

The kawaiiness of the tree is 17.
    
### 2

#### Input

2 2
1 2

#### Output

2

#### Explanation

The kawaiiness of the tree is 2.
  

## Input Format  

- The first line of each test case contains two integers n and k — the number of vertices and the size of the sets to consider.
- The following n-1 lines of each test case describe the tree. Each line contains two integers u and v, indicating an edge between vertices u and v.

## Output Format  

- Return one integer: the kawaiiness of the tree.
  

## Constraints  

- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

depth-first-search, graph, tree, hackwithinfy

## Companies
infosys