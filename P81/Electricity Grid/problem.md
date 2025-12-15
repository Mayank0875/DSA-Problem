## Title
Electricity Grid

## Slug
electricity-grid

## Difficulty
Medium

## Description
Power surges from Plant 1 to Substation n.

The grid has `n` transformers and `m` directed lines. Lines may repeat between the same pair of transformers and self-loops are allowed. A circuit of length `k` is a sequence of exactly `k` directed lines; transformers and lines may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed lines (each line given as two integers `u` `v` meaning a directed line from `u` to `v`), compute the number of distinct circuits that start at transformer 1 and end at transformer `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 transformers. We want the number of directed circuits of length 8 from transformer 1 to transformer 3.
Valid length-8 circuits:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such circuits.

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
Assuming the graph has lines 1->2 and 2->3, the only circuit of length 2 from transformer 1 to transformer 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of transformers, lines, and the required circuit length.
- The next m lines describe the lines. Each line contains two integers u and v, indicating a directed line from transformer u to transformer v.

## Output Format
- Return single integer: the number of circuits modulo 10^9+7.

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
