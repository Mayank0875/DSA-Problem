## Title
Satellite Relay

## Slug
satellite-relay

## Difficulty
Medium

## Description
A signal bounces from Satellite 1 to Ground Station n.

The orbit has `n` satellites and `m` directed beams. Beams may repeat between the same pair of satellites and self-loops are allowed. A relay of length `k` is a sequence of exactly `k` directed beams; satellites and beams may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed beams (each beam given as two integers `u` `v` meaning a directed beam from `u` to `v`), compute the number of distinct relays that start at satellite 1 and end at satellite `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 satellites. We want the number of directed relays of length 8 from satellite 1 to satellite 3.
Valid length-8 relays:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such relays.

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
Assuming the graph has beams 1->2 and 2->3, the only relay of length 2 from satellite 1 to satellite 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of satellites, beams, and the required relay length.
- The next m lines describe the beams. Each line contains two integers u and v, indicating a directed beam from satellite u to satellite v.

## Output Format
- Return single integer: the number of relays modulo 10^9+7.

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
