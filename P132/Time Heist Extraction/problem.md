## Title
Time Heist Extraction

## Slug
time-heist-extraction

## Difficulty
Medium

## Description
Agents are scattered in time. They must all jump to the Extraction Point.

There are $n$ timelines numbered from $1$ to $n$, connected by $n-1$ portals. The network forms a tree structure (there is exactly one path between any two timelines). Currently, all portals are one-way.

The mission clock requires travel to the **Extraction Point (Node 1)**. To ensure success, every other timeline must be able to reach Extraction Point by traveling along the portals in the correct direction.

You are given the current orientation of the portals. Your task is to determine the **minimum** number of portals that need to be re-calibrated so that every timeline can reach Extraction Point.

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
The destination is Extraction Point (1).
- Portal 1->2 points away from 1. Needs calibration.
- Portal 2->4 points away from 1. Needs calibration.
- Portal 3->2 points towards 2 (and effectively towards 1). OK.
- Portal 5->1 points towards 1. OK.
- Portal 5->6 points away from 1 (via 5). Needs calibration.
Total calibrations: 3.

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
Portals 2->3 and 4->5 need to be re-calibrated.

## Input Format
- The first line contains an integer $n$ — the number of timelines.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way portal from timeline $u$ to timeline $v$.

## Output Format
- Return a single integer representing the minimum number of portals that need to be changed.

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
