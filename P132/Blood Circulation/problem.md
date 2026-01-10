## Title
Blood Circulation

## Slug
blood-circulation

## Difficulty
Medium

## Description
A biologist models a vascular system. All veins must return blood to the Heart.

There are $n$ organs numbered from $1$ to $n$, connected by $n-1$ veins. The network forms a tree structure (there is exactly one path between any two organs). Currently, all veins are one-way.

Physiology requires blood to flow to the **Heart (Node 1)**. To ensure success, every other organ must be able to reach Heart by traveling along the veins in the correct direction.

You are given the current orientation of the veins. Your task is to determine the **minimum** number of veins that need to be surgically altered so that every organ can reach Heart.

## Examples

### 1

#### Input
6
1 2
2 4
3 2
5 1
5 6

#### Output
3

#### Explanation
The destination is Heart (1).
- Vein 1->2 points away from 1. Needs alteration.
- Vein 2->4 points away from 1. Needs alteration.
- Vein 3->2 points towards 2 (and effectively towards 1). OK.
- Vein 5->1 points towards 1. OK.
- Vein 5->6 points away from 1 (via 5). Needs alteration.
Total alterations: 3.

### 2

#### Input
5
2 1
2 3
4 3
4 5

#### Output
2

#### Explanation
Veins 2->3 and 4->5 need to be altered.

## Input Format
- The first line contains an integer $n$ — the number of organs.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way vein from organ $u$ to organ $v$.

## Output Format
- Return a single integer representing the minimum number of veins that need to be changed.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ u, v ≤ n
- The graph is guaranteed to be a tree.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
tree, depth-first-search, breadth-first-search, graph

## Company
google, amazon
