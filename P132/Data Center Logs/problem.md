## Title
Data Center Logs

## Slug
data-center-logs

## Difficulty
Medium

## Description
A server farm collects logs. All servers must send their log files to the Master Logger.

There are $n$ servers numbered from $1$ to $n$, connected by $n-1$ fiber cables. The network forms a tree structure (there is exactly one path between any two servers). Currently, all fiber cables are one-way.

The system requires all data to route to the **Master Logger (Node 1)**. To ensure success, every other server must be able to reach Master Logger by traveling along the fiber cables in the correct direction.

You are given the current orientation of the fiber cables. Your task is to determine the **minimum** number of fiber cables that need to be reconfigured so that every server can reach Master Logger.

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
The destination is Master Logger (1).
- Cable 1->2 points away from 1. Needs reconfiguration.
- Cable 2->4 points away from 1. Needs reconfiguration.
- Cable 3->2 points towards 2 (and effectively towards 1). OK.
- Cable 5->1 points towards 1. OK.
- Cable 5->6 points away from 1 (via 5). Needs reconfiguration.
Total reconfigurations: 3.

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
Cables 2->3 and 4->5 need to be reconfigured.

## Input Format
- The first line contains an integer $n$ — the number of servers.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way fiber cable from server $u$ to server $v$.

## Output Format
- Return a single integer representing the minimum number of fiber cables that need to be changed.

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
