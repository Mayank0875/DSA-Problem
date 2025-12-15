## Title
Manufacturing Assembly

## Slug
manufacturing-assembly

## Difficulty
Medium

## Description
A part moves from Station 1 to Assembly n.

The factory has `n` stations and `m` directed conveyor belts. Conveyor belts may repeat between the same pair of stations and self-loops are allowed. A process line of length `k` is a sequence of exactly `k` directed conveyor belts; stations and conveyor belts may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed conveyor belts (each conveyor belt given as two integers `u` `v` meaning a directed conveyor belt from `u` to `v`), compute the number of distinct process lines that start at station 1 and end at station `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 stations. We want the number of directed process lines of length 8 from station 1 to station 3.
Valid length-8 process lines:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such process lines.

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
Assuming the graph has conveyor belts 1->2 and 2->3, the only process line of length 2 from station 1 to station 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of stations, conveyor belts, and the required process line length.
- The next m lines describe the conveyor belts. Each line contains two integers u and v, indicating a directed conveyor belt from station u to station v.

## Output Format
- Return single integer: the number of process lines modulo 10^9+7.

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
