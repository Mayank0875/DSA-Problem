## Title
Water Park Slides

## Slug
water-park-slides

## Difficulty
Medium

## Description
A tuber slides from the Top Tower (node 1) to the Main Pool (node n).

The water park has `n` pools and `m` directed slides. Slides may repeat between the same pair of pools and self-loops are allowed. A descent of length `k` is a sequence of exactly `k` directed slides; pools and slides may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed slides (each slide given as two integers `u` `v` meaning a directed slide from `u` to `v`), compute the number of distinct descents that start at pool 1 and end at pool `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 pools. We want the number of directed descents of length 8 from pool 1 to pool 3.
Valid length-8 descents:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such descents.

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
Assuming the graph has slides 1->2 and 2->3, the only descent of length 2 from pool 1 to pool 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of pools, slides, and the required descent length.
- The next m lines describe the slides. Each line contains two integers u and v, indicating a directed slide from pool u to pool v.

## Output Format
- Return single integer: the number of descents modulo 10^9+7.

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
