## Title
Energy Grid

## Slug
energy-grid

## Difficulty
Medium

## Description
A solar farm network collects power. All current must flow into the Main Battery Bank.

There are $n$ solar arrays numbered from $1$ to $n$, connected by $n-1$ power lines. The network forms a tree structure (there is exactly one path between any two solar arrays). Currently, all power lines are one-way.

Efficiency dictates power moves to the **Main Battery (Node 1)**. To ensure success, every other solar array must be able to reach Main Battery by traveling along the power lines in the correct direction.

You are given the current orientation of the power lines. Your task is to determine the **minimum** number of power lines that need to be rewired so that every solar array can reach Main Battery.

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
The destination is Main Battery (1).
- Line 1->2 points away from 1. Needs rewiring.
- Line 2->4 points away from 1. Needs rewiring.
- Line 3->2 points towards 2 (and effectively towards 1). OK.
- Line 5->1 points towards 1. OK.
- Line 5->6 points away from 1 (via 5). Needs rewiring.
Total rewirings: 3.

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
Lines 2->3 and 4->5 need to be rewired.

## Input Format
- The first line contains an integer $n$ — the number of solar arrays.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way power line from solar array $u$ to solar array $v$.

## Output Format
- Return a single integer representing the minimum number of power lines that need to be changed.

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
