## Title
Logistics Supply Chain

## Slug
logistics-supply-chain

## Difficulty
Medium

## Description
Goods move from Factory (node 1) to Retail Store (node n).

The supply chain has `n` warehouses and `m` directed truck routes. Truck routes may repeat between the same pair of warehouses and self-loops are allowed. A shipment of length `k` is a sequence of exactly `k` directed truck routes; warehouses and truck routes may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed truck routes (each truck route given as two integers `u` `v` meaning a directed truck route from `u` to `v`), compute the number of distinct shipments that start at warehouse 1 and end at warehouse `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 warehouses. We want the number of directed shipments of length 8 from warehouse 1 to warehouse 3.
Valid length-8 shipments:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such shipments.

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
Assuming the graph has truck routes 1->2 and 2->3, the only shipment of length 2 from warehouse 1 to warehouse 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of warehouses, truck routes, and the required shipment length.
- The next m lines describe the truck routes. Each line contains two integers u and v, indicating a directed truck route from warehouse u to warehouse v.

## Output Format
- Return single integer: the number of shipments modulo 10^9+7.

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
