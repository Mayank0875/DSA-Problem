## Title
Elevator System

## Slug
elevator-system

## Difficulty
Medium

## Description
A person moves from Floor 1 to Floor n.

The skyscraper has `n` floors and `m` directed elevator rides. Elevator rides may repeat between the same pair of floors and self-loops are allowed. A trip of length `k` is a sequence of exactly `k` directed elevator rides; floors and elevator rides may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed elevator rides (each elevator ride given as two integers `u` `v` meaning a directed elevator ride from `u` to `v`), compute the number of distinct trips that start at floor 1 and end at floor `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 floors. We want the number of directed trips of length 8 from floor 1 to floor 3.
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
Assuming the graph has elevator rides 1->2 and 2->3, the only trip of length 2 from floor 1 to floor 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of floors, elevator rides, and the required trip length.
- The next m lines describe the elevator rides. Each line contains two integers u and v, indicating a directed elevator ride from floor u to floor v.

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
