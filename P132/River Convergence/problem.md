## Title
River Convergence

## Slug
river-convergence

## Difficulty
Medium

## Description
A hydrologist analyzes a river system. All tributaries must eventually flow into the Main Reservoir.

There are $n$ monitoring stations numbered from $1$ to $n$, connected by $n-1$ river segments. The network forms a tree structure (there is exactly one path between any two monitoring stations). Currently, all river segments are one-way.

The goal is to direct all water flow to the **Main Reservoir (Node 1)**. To ensure success, every other station must be able to reach Main Reservoir by traveling along the river segments in the correct direction.

You are given the current orientation of the river segments. Your task is to determine the **minimum** number of river segments that need to be reversed (by terraforming) so that every station can reach Main Reservoir.

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
The destination is Main Reservoir (1).
- Segment 1->2 points away from 1. Needs reversal.
- Segment 2->4 points away from 1. Needs reversal.
- Segment 3->2 points towards 2 (and effectively towards 1). OK.
- Segment 5->1 points towards 1. OK.
- Segment 5->6 points away from 1 (via 5). Needs reversal.
Total reversals: 3.

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
Segments 2->3 and 4->5 need to be reversed.

## Input Format
- The first line contains an integer $n$ — the number of monitoring stations.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way river segment from station $u$ to station $v$.

## Output Format
- Return a single integer representing the minimum number of river segments that need to be changed.

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
