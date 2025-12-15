## Title
Laser Reflection

## Slug
laser-reflection

## Difficulty
Medium

## Description
A laser beam bounces from Mirror 1 to Detector n.

The optical table has `n` mirrors and `m` directed beams. Beams may repeat between the same pair of mirrors and self-loops are allowed. A reflection path of length `k` is a sequence of exactly `k` directed beams; mirrors and beams may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed beams (each beam given as two integers `u` `v` meaning a directed beam from `u` to `v`), compute the number of distinct reflection paths that start at mirror 1 and end at mirror `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 mirrors. We want the number of directed reflection paths of length 8 from mirror 1 to mirror 3.
Valid length-8 reflection paths:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such reflection paths.

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
Assuming the graph has beams 1->2 and 2->3, the only reflection path of length 2 from mirror 1 to mirror 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of mirrors, beams, and the required reflection path length.
- The next m lines describe the beams. Each line contains two integers u and v, indicating a directed beam from mirror u to mirror v.

## Output Format
- Return single integer: the number of reflection paths modulo 10^9+7.

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
