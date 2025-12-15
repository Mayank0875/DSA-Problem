## Title
Teleporter Maze

## Slug
teleporter-maze

## Difficulty
Medium

## Description
A test subject warps from Chamber 1 to Exit n.

The lab has `n` chambers and `m` directed teleporters. Teleporters may repeat between the same pair of chambers and self-loops are allowed. A solution of length `k` is a sequence of exactly `k` directed teleporters; chambers and teleporters may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed teleporters (each teleporter given as two integers `u` `v` meaning a directed teleporter from `u` to `v`), compute the number of distinct solutions that start at chamber 1 and end at chamber `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 chambers. We want the number of directed solutions of length 8 from chamber 1 to chamber 3.
Valid length-8 solutions:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such solutions.

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
Assuming the graph has teleporters 1->2 and 2->3, the only solution of length 2 from chamber 1 to chamber 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of chambers, teleporters, and the required solution length.
- The next m lines describe the teleporters. Each line contains two integers u and v, indicating a directed teleporter from chamber u to chamber v.

## Output Format
- Return single integer: the number of solutions modulo 10^9+7.

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
