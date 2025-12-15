## Title
Postal Sorting

## Slug
postal-sorting

## Difficulty
Medium

## Description
A letter moves from Drop Box 1 to Mailbox n.

The postal service has `n` sorting centers and `m` directed trucks. Trucks may repeat between the same pair of sorting centers and self-loops are allowed. A delivery route of length `k` is a sequence of exactly `k` directed trucks; sorting centers and trucks may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed trucks (each truck given as two integers `u` `v` meaning a directed truck from `u` to `v`), compute the number of distinct delivery routes that start at sorting center 1 and end at sorting center `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 sorting centers. We want the number of directed delivery routes of length 8 from sorting center 1 to sorting center 3.
Valid length-8 delivery routes:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such delivery routes.

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
Assuming the graph has trucks 1->2 and 2->3, the only delivery route of length 2 from sorting center 1 to sorting center 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of sorting centers, trucks, and the required delivery route length.
- The next m lines describe the trucks. Each line contains two integers u and v, indicating a directed truck from sorting center u to sorting center v.

## Output Format
- Return single integer: the number of delivery routes modulo 10^9+7.

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
