## Title
Dungeon Crawler

## Slug
dungeon-crawler

## Difficulty
Medium

## Description
An adventurer moves from the Entrance (node 1) to the Boss Room (node n).

The dungeon has `n` rooms and `m` directed doors. Doors may repeat between the same pair of rooms and self-loops are allowed. A run of length `k` is a sequence of exactly `k` directed doors; rooms and doors may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed doors (each door given as two integers `u` `v` meaning a directed door from `u` to `v`), compute the number of distinct runs that start at room 1 and end at room `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 rooms. We want the number of directed runs of length 8 from room 1 to room 3.
Valid length-8 runs:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such runs.

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
Assuming the graph has doors 1->2 and 2->3, the only run of length 2 from room 1 to room 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of rooms, doors, and the required run length.
- The next m lines describe the doors. Each line contains two integers u and v, indicating a directed door from room u to room v.

## Output Format
- Return single integer: the number of runs modulo 10^9+7.

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
