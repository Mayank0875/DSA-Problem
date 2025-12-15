## Title
Ant Colony Foraging

## Slug
ant-colony-foraging

## Difficulty
Medium

## Description
An ant moves from the Nest Entrance (node 1) to the Food Store (node n).

The colony has `n` chambers and `m` directed tunnels. Tunnels may repeat between the same pair of chambers and self-loops are allowed. A walk of length `k` is a sequence of exactly `k` directed tunnels; chambers and tunnels may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed tunnels (each tunnel given as two integers `u` `v` meaning a directed tunnel from `u` to `v`), compute the number of distinct walks that start at chamber 1 and end at chamber `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 chambers. We want the number of directed walks of length 8 from chamber 1 to chamber 3.
Valid length-8 walks:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such walks.

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
Assuming the graph has tunnels 1->2 and 2->3, the only walk of length 2 from chamber 1 to chamber 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of chambers, tunnels, and the required walk length.
- The next m lines describe the tunnels. Each line contains two integers u and v, indicating a directed tunnel from chamber u to chamber v.

## Output Format
- Return single integer: the number of walks modulo 10^9+7.

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
