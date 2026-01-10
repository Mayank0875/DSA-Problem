## Title
Pilgrimage Route

## Slug
pilgrimage-route

## Difficulty
Medium

## Description
Pilgrims travel between shrines. All paths must guide the faithful to the Grand Temple.

There are $n$ shrines numbered from $1$ to $n$, connected by $n-1$ paths. The network forms a tree structure (there is exactly one path between any two shrines). Currently, all paths are one-way.

Tradition dictates all journeys end to the **Grand Temple (Node 1)**. To ensure success, every other shrine must be able to reach Grand Temple by traveling along the paths in the correct direction.

You are given the current orientation of the paths. Your task is to determine the **minimum** number of paths that need to be signposted differently so that every shrine can reach Grand Temple.

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
The destination is Grand Temple (1).
- Path 1->2 points away from 1. Needs sign change.
- Path 2->4 points away from 1. Needs sign change.
- Path 3->2 points towards 2 (and effectively towards 1). OK.
- Path 5->1 points towards 1. OK.
- Path 5->6 points away from 1 (via 5). Needs sign change.
Total sign changes: 3.

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
Paths 2->3 and 4->5 need to be changed.

## Input Format
- The first line contains an integer $n$ — the number of shrines.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way path from shrine $u$ to shrine $v$.

## Output Format
- Return a single integer representing the minimum number of paths that need to be changed.

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
