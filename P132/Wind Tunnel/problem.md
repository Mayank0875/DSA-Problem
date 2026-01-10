## Title
Wind Tunnel

## Slug
wind-tunnel

## Difficulty
Medium

## Description
Air flows through ducts. All air must be directed to the Main Turbine.

There are $n$ chambers numbered from $1$ to $n$, connected by $n-1$ ducts. The network forms a tree structure (there is exactly one path between any two chambers). Currently, all ducts are one-way.

Aerodynamics require flow to the **Main Turbine (Node 1)**. To ensure success, every other chamber must be able to reach Main Turbine by traveling along the ducts in the correct direction.

You are given the current orientation of the ducts. Your task is to determine the **minimum** number of ducts that need to be angled so that every chamber can reach Main Turbine.

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
The destination is Main Turbine (1).
- Duct 1->2 points away from 1. Needs angle change.
- Duct 2->4 points away from 1. Needs angle change.
- Duct 3->2 points towards 2 (and effectively towards 1). OK.
- Duct 5->1 points towards 1. OK.
- Duct 5->6 points away from 1 (via 5). Needs angle change.
Total angle changes: 3.

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
Ducts 2->3 and 4->5 need to be angled.

## Input Format
- The first line contains an integer $n$ — the number of chambers.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way duct from chamber $u$ to chamber $v$.

## Output Format
- Return a single integer representing the minimum number of ducts that need to be changed.

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
