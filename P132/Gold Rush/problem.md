## Title
Gold Rush

## Slug
gold-rush

## Difficulty
Medium

## Description
Miners find gold. All nuggets must be transported to the Bank.

There are $n$ claims numbered from $1$ to $n$, connected by $n-1$ wagon trails. The network forms a tree structure (there is exactly one path between any two claims). Currently, all wagon trails are one-way.

Wealth flows to the **Bank (Node 1)**. To ensure success, every other claim must be able to reach Bank by traveling along the wagon trails in the correct direction.

You are given the current orientation of the wagon trails. Your task is to determine the **minimum** number of wagon trails that need to be redirected so that every claim can reach Bank.

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
The destination is Bank (1).
- Trail 1->2 points away from 1. Needs redirection.
- Trail 2->4 points away from 1. Needs redirection.
- Trail 3->2 points towards 2 (and effectively towards 1). OK.
- Trail 5->1 points towards 1. OK.
- Trail 5->6 points away from 1 (via 5). Needs redirection.
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
Trails 2->3 and 4->5 need to be redirected.

## Input Format
- The first line contains an integer $n$ — the number of claims.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way wagon trail from claim $u$ to claim $v$.

## Output Format
- Return a single integer representing the minimum number of wagon trails that need to be changed.

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
