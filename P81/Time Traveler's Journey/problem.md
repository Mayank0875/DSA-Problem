## Title
Time Traveler's Journey

## Slug
time-travelers-journey

## Difficulty
Medium

## Description
A traveler jumps from the Past (node 1) to the Future (node n) through temporal rifts.

The timeline has `n` eras and `m` directed rifts. Rifts may repeat between the same pair of eras and self-loops are allowed. A timeline of length `k` is a sequence of exactly `k` directed rifts; eras and rifts may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed rifts (each rift given as two integers `u` `v` meaning a directed rift from `u` to `v`), compute the number of distinct timelines that start at era 1 and end at era `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 eras. We want the number of directed timelines of length 8 from era 1 to era 3.
Valid length-8 timelines:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such timelines.

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
Assuming the graph has rifts 1->2 and 2->3, the only timeline of length 2 from era 1 to era 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of eras, rifts, and the required timeline length.
- The next m lines describe the rifts. Each line contains two integers u and v, indicating a directed rift from era u to era v.

## Output Format
- Return single integer: the number of timelines modulo 10^9+7.

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
