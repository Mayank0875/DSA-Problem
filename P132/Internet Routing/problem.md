## Title
Internet Routing

## Slug
internet-routing

## Difficulty
Medium

## Description
Packets traverse a mesh. All traffic must reach the ISP Gateway.

There are $n$ routers numbered from $1$ to $n$, connected by $n-1$ links. The network forms a tree structure (there is exactly one path between any two routers). Currently, all links are one-way.

Routing tables direct traffic to the **ISP Gateway (Node 1)**. To ensure success, every other router must be able to reach ISP Gateway by traveling along the links in the correct direction.

You are given the current orientation of the links. Your task is to determine the **minimum** number of links that need to be updated so that every router can reach ISP Gateway.

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
The destination is ISP Gateway (1).
- Link 1->2 points away from 1. Needs update.
- Link 2->4 points away from 1. Needs update.
- Link 3->2 points towards 2 (and effectively towards 1). OK.
- Link 5->1 points towards 1. OK.
- Link 5->6 points away from 1 (via 5). Needs update.
Total updates: 3.

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
Links 2->3 and 4->5 need to be updated.

## Input Format
- The first line contains an integer $n$ — the number of routers.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way link from router $u$ to router $v$.

## Output Format
- Return a single integer representing the minimum number of links that need to be changed.

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
