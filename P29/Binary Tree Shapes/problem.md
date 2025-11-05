## Title

Binary Tree Shapes

## Slug

binary-tree-shapes

## Difficulty

Easy

## Description

You are investigating the structures of binary trees. The number of different binary trees you can form with $n$ nodes is a known problem. A related problem is counting 'full' binary trees. How many different shapes of full binary trees can you form using exactly $n$ 'internal' nodes (nodes with children)? This count is surprisingly related to parentheses!
## Examples

### 1

#### Input

3

#### Output

5

#### Explanation

The 5 unique well-formed combinations are:
((()))
(()())
(())()
()(())
()()()

### 2

#### Input

1

#### Output

1

#### Explanation
The only combination is ().

## Input Format  

- The input consists of a single line containing one integer, `n`.

## Output Format  

- Return single integer representing total number of well-formed parenthesis combinations.
  

## Constraints  

- 1 ≤ n ≤ 8

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

backtracking, recursion