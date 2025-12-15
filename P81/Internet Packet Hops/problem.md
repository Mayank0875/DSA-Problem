## Title
Internet Packet Hops

## Slug
internet-packet-hops

## Difficulty
Medium

## Description
A packet routes from Client (node 1) to Server (node n).

The internet has `n` routers and `m` directed cables. Cables may repeat between the same pair of routers and self-loops are allowed. A route of length `k` is a sequence of exactly `k` directed cables; routers and cables may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed cables (each cable given as two integers `u` `v` meaning a directed cable from `u` to `v`), compute the number of distinct routes that start at router 1 and end at router `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 routers. We want the number of directed routes of length 8 from router 1 to router 3.
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
Assuming the graph has cables 1->2 and 2->3, the only route of length 2 from router 1 to router 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of routers, cables, and the required route length.
- The next m lines describe the cables. Each line contains two integers u and v, indicating a directed cable from router u to router v.

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
