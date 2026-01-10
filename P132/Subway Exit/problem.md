## Title
Subway Exit

## Slug
subway-exit

## Difficulty
Medium

## Description
A concert ends. The crowd flows through corridors to the Main Exit.

There are $n$ halls numbered from $1$ to $n$, connected by $n-1$ corridors. The network forms a tree structure (there is exactly one path between any two halls). Currently, all corridors are one-way.

Crowd control directs people to the **Main Exit (Node 1)**. To ensure success, every other hall must be able to reach Main Exit by traveling along the corridors in the correct direction.

You are given the current orientation of the corridors. Your task is to determine the **minimum** number of corridors that need to be barricaded differently so that every hall can reach Main Exit.

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
The destination is Main Exit (1).
- Corridor 1->2 points away from 1. Needs change.
- Corridor 2->4 points away from 1. Needs change.
- Corridor 3->2 points towards 2 (and effectively towards 1). OK.
- Corridor 5->1 points towards 1. OK.
- Corridor 5->6 points away from 1 (via 5). Needs change.
Total changes: 3.

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
Corridors 2->3 and 4->5 need to be changed.

## Input Format
- The first line contains an integer $n$ — the number of halls.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way corridor from hall $u$ to hall $v$.

## Output Format
- Return a single integer representing the minimum number of corridors that need to be changed.

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
