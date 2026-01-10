## Title
The Great Gathering

## Slug
the-great-gathering

## Difficulty
Medium

## Description
Clans are scattered across islands connected by bridges. Everyone must travel to the Gathering Hall.

There are $n$ islands numbered from $1$ to $n$, connected by $n-1$ bridges. The network forms a tree structure (there is exactly one path between any two islands). Currently, all bridges are one-way.

The summons calls everyone to the **Gathering Hall (Node 1)**. To ensure success, every other island must be able to reach Gathering Hall by traveling along the bridges in the correct direction.

You are given the current orientation of the bridges. Your task is to determine the **minimum** number of bridges that need to be rebuilt so that every island can reach Gathering Hall.

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
The destination is Gathering Hall (1).
- Bridge 1->2 points away from 1. Needs rebuild.
- Bridge 2->4 points away from 1. Needs rebuild.
- Bridge 3->2 points towards 2 (and effectively towards 1). OK.
- Bridge 5->1 points towards 1. OK.
- Bridge 5->6 points away from 1 (via 5). Needs rebuild.
Total rebuilds: 3.

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
Bridges 2->3 and 4->5 need to be rebuilt.

## Input Format
- The first line contains an integer $n$ — the number of islands.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way bridge from island $u$ to island $v$.

## Output Format
- Return a single integer representing the minimum number of bridges that need to be changed.

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
