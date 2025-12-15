## Title
Water Pipeline

## Slug
water-pipeline

## Difficulty
Medium

## Description
Water flows from Reservoir 1 to Treatment Plant n.

The utility has `n` valves and `m` directed pipes. Pipes may repeat between the same pair of valves and self-loops are allowed. A flow path of length `k` is a sequence of exactly `k` directed pipes; valves and pipes may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed pipes (each pipe given as two integers `u` `v` meaning a directed pipe from `u` to `v`), compute the number of distinct flow paths that start at valve 1 and end at valve `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 valves. We want the number of directed flow paths of length 8 from valve 1 to valve 3.
Valid length-8 flow paths:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such flow paths.

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
Assuming the graph has pipes 1->2 and 2->3, the only flow path of length 2 from valve 1 to valve 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of valves, pipes, and the required flow path length.
- The next m lines describe the pipes. Each line contains two integers u and v, indicating a directed pipe from valve u to valve v.

## Output Format
- Return single integer: the number of flow paths modulo 10^9+7.

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
