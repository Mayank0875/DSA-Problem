## Title
Bee Pollination

## Slug
bee-pollination

## Difficulty
Medium

## Description
A bee flies from Flower 1 to Flower n.

The garden has `n` flowers and `m` directed flights. Flights may repeat between the same pair of flowers and self-loops are allowed. A forage route of length `k` is a sequence of exactly `k` directed flights; flowers and flights may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed flights (each flight given as two integers `u` `v` meaning a directed flight from `u` to `v`), compute the number of distinct forage routes that start at flower 1 and end at flower `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 flowers. We want the number of directed forage routes of length 8 from flower 1 to flower 3.
Valid length-8 forage routes:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such forage routes.

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
Assuming the graph has flights 1->2 and 2->3, the only forage route of length 2 from flower 1 to flower 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of flowers, flights, and the required forage route length.
- The next m lines describe the flights. Each line contains two integers u and v, indicating a directed flight from flower u to flower v.

## Output Format
- Return single integer: the number of forage routes modulo 10^9+7.

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
