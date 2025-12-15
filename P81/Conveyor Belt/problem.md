## Title
Conveyor Belt

## Slug
conveyor-belt

## Difficulty
Medium

## Description
An item moves from Intake 1 to Shipping n.

The warehouse has `n` sorters and `m` directed belts. Belts may repeat between the same pair of sorters and self-loops are allowed. A track of length `k` is a sequence of exactly `k` directed belts; sorters and belts may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed belts (each belt given as two integers `u` `v` meaning a directed belt from `u` to `v`), compute the number of distinct tracks that start at sorter 1 and end at sorter `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 sorters. We want the number of directed tracks of length 8 from sorter 1 to sorter 3.
Valid length-8 tracks:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such tracks.

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
Assuming the graph has belts 1->2 and 2->3, the only track of length 2 from sorter 1 to sorter 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of sorters, belts, and the required track length.
- The next m lines describe the belts. Each line contains two integers u and v, indicating a directed belt from sorter u to sorter v.

## Output Format
- Return single integer: the number of tracks modulo 10^9+7.

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
