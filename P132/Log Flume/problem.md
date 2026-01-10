## Title
Log Flume

## Slug
log-flume

## Difficulty
Medium

## Description
Logs float down canals. They must all arrive at the Sawmill.

There are $n$ checkpoints numbered from $1$ to $n$, connected by $n-1$ canals. The network forms a tree structure (there is exactly one path between any two checkpoints). Currently, all canals are one-way.

The current carries logs to the **Sawmill (Node 1)**. To ensure success, every other checkpoint must be able to reach Sawmill by traveling along the canals in the correct direction.

You are given the current orientation of the canals. Your task is to determine the **minimum** number of canals that need to be pumped backwards so that every checkpoint can reach Sawmill.

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
The destination is Sawmill (1).
- Canal 1->2 points away from 1. Needs pumping.
- Canal 2->4 points away from 1. Needs pumping.
- Canal 3->2 points towards 2 (and effectively towards 1). OK.
- Canal 5->1 points towards 1. OK.
- Canal 5->6 points away from 1 (via 5). Needs pumping.
Total pumpings: 3.

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
Canals 2->3 and 4->5 need to be pumped.

## Input Format
- The first line contains an integer $n$ — the number of checkpoints.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way canal from checkpoint $u$ to checkpoint $v$.

## Output Format
- Return a single integer representing the minimum number of canals that need to be changed.

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
