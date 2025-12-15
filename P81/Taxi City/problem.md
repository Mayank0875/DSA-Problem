## Title
Taxi City

## Slug
taxi-city

## Difficulty
Medium

## Description
A taxi drives from Intersection 1 to Intersection n.

The city grid has `n` intersections and `m` directed roads. Roads may repeat between the same pair of intersections and self-loops are allowed. A trip of length `k` is a sequence of exactly `k` directed roads; intersections and roads may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed roads (each road given as two integers `u` `v` meaning a directed road from `u` to `v`), compute the number of distinct trips that start at intersection 1 and end at intersection `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 intersections. We want the number of directed trips of length 8 from intersection 1 to intersection 3.
Valid length-8 trips:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such trips.

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
Assuming the graph has roads 1->2 and 2->3, the only trip of length 2 from intersection 1 to intersection 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of intersections, roads, and the required trip length.
- The next m lines describe the roads. Each line contains two integers u and v, indicating a directed road from intersection u to intersection v.

## Output Format
- Return single integer: the number of trips modulo 10^9+7.

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
