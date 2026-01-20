## Title

Rae's Rare Trees

## Slug

raes-rare-trees

## Difficulty

Medium

## Description

As an Earth mage, Rae has mastered the spell of growing trees! But Manaria brags that she can grow a more impressive species of trees. Rae remembers that the most rare type of tree can be grown using a formula represented by a certain permutation — please help her construct it!

You are given a permutation $p$ of length $n$.

Determine if there exists an undirected tree with $n$ vertices labeled $1, 2, \dots, n$, satisfying the following condition:

Let $u$ and $v$ ($1 \le u < v \le n$) be any two vertices connected by an edge. Then $u$ appears before $v$ in $p$.

## Examples

### 1

#### Input

6
1 3 4 5 2 6

#### Output

True

#### Explanation

We can construct the tree with edges $\{1,3\}, \{1,4\}, \{5,6\}, \{2,6\}, \{1,6\}$.
Checking the condition for $\{1,3\}$: $1<3$ and 1 appears before 3.
Checking the condition for $\{2,6\}$: $2<6$ and 2 appears before 6 (2 is at index 4, 6 is at index 5).
    
### 2

#### Input

4
3 4 1 2

#### Output

False

#### Explanation

It can be shown that no such tree exists.

## Input Format  

- The first line has an integer n.
- The second line of contains $n$ integers, $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$). It is guaranteed that all $p_i$ are distinct.

## Output Format  

- Return on a single line "True" if there exists a tree satisfying the given condition, and "False" otherwise.
  

## Constraints  

- 1 ≤ n ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, graph, breadth-first-search, depth-first-search

## Company
google