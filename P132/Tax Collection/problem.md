## Title
Tax Collection

## Slug
tax-collection

## Difficulty
Medium

## Description
Gold flows from provinces. All taxes must reach the Royal Treasury.

There are $n$ towns numbered from $1$ to $n$, connected by $n-1$ trade routes. The network forms a tree structure (there is exactly one path between any two towns). Currently, all trade routes are one-way.

The King demands gold flow to the **Royal Treasury (Node 1)**. To ensure success, every other town must be able to reach Royal Treasury by traveling along the trade routes in the correct direction.

You are given the current orientation of the trade routes. Your task is to determine the **minimum** number of trade routes that need to be enforced differently so that every town can reach Royal Treasury.

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
The destination is Royal Treasury (1).
- Route 1->2 points away from 1. Needs enforcement.
- Route 2->4 points away from 1. Needs enforcement.
- Route 3->2 points towards 2 (and effectively towards 1). OK.
- Route 5->1 points towards 1. OK.
- Route 5->6 points away from 1 (via 5). Needs enforcement.
Total enforcements: 3.

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
Routes 2->3 and 4->5 need to be enforced.

## Input Format
- The first line contains an integer $n$ — the number of towns.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way trade route from town $u$ to town $v$.

## Output Format
- Return a single integer representing the minimum number of trade routes that need to be changed.

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
