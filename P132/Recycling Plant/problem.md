## Title
Recycling Plant

## Slug
recycling-plant

## Difficulty
Medium

## Description
Waste moves through chutes. All recyclable material must reach the Baler.

There are $n$ sorting stations numbered from $1$ to $n$, connected by $n-1$ chutes. The network forms a tree structure (there is exactly one path between any two sorting stations). Currently, all chutes are one-way.

Gravity feeds material to the **Baler (Node 1)**. To ensure success, every other station must be able to reach Baler by traveling along the chutes in the correct direction.

You are given the current orientation of the chutes. Your task is to determine the **minimum** number of chutes that need to be redirected so that every station can reach Baler.

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
The destination is Baler (1).
- Chute 1->2 points away from 1. Needs redirection.
- Chute 2->4 points away from 1. Needs redirection.
- Chute 3->2 points towards 2 (and effectively towards 1). OK.
- Chute 5->1 points towards 1. OK.
- Chute 5->6 points away from 1 (via 5). Needs redirection.
Total redirections: 3.

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
Chutes 2->3 and 4->5 need to be redirected.

## Input Format
- The first line contains an integer $n$ — the number of sorting stations.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way chute from station $u$ to station $v$.

## Output Format
- Return a single integer representing the minimum number of chutes that need to be changed.

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
