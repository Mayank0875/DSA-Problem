## Title
Mall Escalators

## Slug
mall-escalators

## Difficulty
Medium

## Description
A mall is closing. All escalators must be set to bring customers to the Main Exit.

There are $n$ floors/zones numbered from $1$ to $n$, connected by $n-1$ escalators. The network forms a tree structure (there is exactly one path between any two floors/zones). Currently, all escalators are one-way.

Closing procedures require movement to the **Main Exit (Node 1)**. To ensure success, every other floor/zone must be able to reach Main Exit by traveling along the escalators in the correct direction.

You are given the current orientation of the escalators. Your task is to determine the **minimum** number of escalators that need to be switched so that every floor/zone can reach Main Exit.

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
- Escalator 1->2 points away from 1. Needs switch.
- Escalator 2->4 points away from 1. Needs switch.
- Escalator 3->2 points towards 2 (and effectively towards 1). OK.
- Escalator 5->1 points towards 1. OK.
- Escalator 5->6 points away from 1 (via 5). Needs switch.
Total switchs: 3.

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
Escalators 2->3 and 4->5 need to be switched.

## Input Format
- The first line contains an integer $n$ — the number of floors/zones.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way escalator from floor/zone $u$ to floor/zone $v$.

## Output Format
- Return a single integer representing the minimum number of escalators that need to be changed.

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
