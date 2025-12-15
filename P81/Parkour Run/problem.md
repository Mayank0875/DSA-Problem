## Title
Parkour Run

## Slug
parkour-run

## Difficulty
Medium

## Description
A freerunner jumps from Rooftop 1 to Rooftop n.

The skyline has `n` rooftops and `m` directed jumps. Jumps may repeat between the same pair of rooftops and self-loops are allowed. A run of length `k` is a sequence of exactly `k` directed jumps; rooftops and jumps may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed jumps (each jump given as two integers `u` `v` meaning a directed jump from `u` to `v`), compute the number of distinct runs that start at rooftop 1 and end at rooftop `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 rooftops. We want the number of directed runs of length 8 from rooftop 1 to rooftop 3.
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
Assuming the graph has jumps 1->2 and 2->3, the only run of length 2 from rooftop 1 to rooftop 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of rooftops, jumps, and the required run length.
- The next m lines describe the jumps. Each line contains two integers u and v, indicating a directed jump from rooftop u to rooftop v.

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
