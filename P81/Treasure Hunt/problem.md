## Title
Treasure Hunt

## Slug
treasure-hunt

## Difficulty
Medium

## Description
A hunter follows clues from Location 1 to Location n.

The island has `n` landmarks and `m` directed clues. Clues may repeat between the same pair of landmarks and self-loops are allowed. A trail of length `k` is a sequence of exactly `k` directed clues; landmarks and clues may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed clues (each clue given as two integers `u` `v` meaning a directed clue from `u` to `v`), compute the number of distinct trails that start at landmark 1 and end at landmark `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 landmarks. We want the number of directed trails of length 8 from landmark 1 to landmark 3.
Valid length-8 trails:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such trails.

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
Assuming the graph has clues 1->2 and 2->3, the only trail of length 2 from landmark 1 to landmark 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of landmarks, clues, and the required trail length.
- The next m lines describe the clues. Each line contains two integers u and v, indicating a directed clue from landmark u to landmark v.

## Output Format
- Return single integer: the number of trails modulo 10^9+7.

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
