## Title
Robot Patrol Route

## Slug
robot-patrol-route

## Difficulty
Medium

## Description
A security robot needs to move from the Charging Station (node 1) to the Control Room (node n).

The facility has `n` waypoints and `m` directed paths. Paths may repeat between the same pair of waypoints and self-loops are allowed. A route of length `k` is a sequence of exactly `k` directed paths; waypoints and paths may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed paths (each path given as two integers `u` `v` meaning a directed path from `u` to `v`), compute the number of distinct routes that start at waypoint 1 and end at waypoint `n` with length exactly `k`. Output the answer modulo 1000000007.

## Examples

### 1

#### Input
3 4 8
1 2
2 3
3 1
3 2

#### Output
2

#### Explanation
We have 3 waypoints. We want the number of directed routes of length 8 from waypoint 1 to waypoint 3.
Valid length-8 routes:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such routes.

### 2

#### Input
3 4 2
1 2
2 3
3 1
3 2

#### Output
1

#### Explanation
Assuming the graph has paths 1->2 and 2->3, the only route of length 2 from waypoint 1 to waypoint 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of waypoints, paths, and the required route length.
- The next m lines describe the paths. Each line contains two integers u and v, indicating a directed path from waypoint u to waypoint v.

## Output Format
- Return single integer: the number of routes modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ 10^5
- 1 ≤ k ≤ 10^18
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
