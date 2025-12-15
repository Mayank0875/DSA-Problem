## Title
Relay Race

## Slug
relay-race

## Difficulty
Medium

## Description
A baton is passed from Runner 1 to Runner n.

The track team has `n` runners and `m` directed handoffs. Handoffs may repeat between the same pair of runners and self-loops are allowed. A race sequence of length `k` is a sequence of exactly `k` directed handoffs; runners and handoffs may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed handoffs (each handoff given as two integers `u` `v` meaning a directed handoff from `u` to `v`), compute the number of distinct race sequences that start at runner 1 and end at runner `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 runners. We want the number of directed race sequences of length 8 from runner 1 to runner 3.
Valid length-8 race sequences:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such race sequences.

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
Assuming the graph has handoffs 1->2 and 2->3, the only race sequence of length 2 from runner 1 to runner 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of runners, handoffs, and the required race sequence length.
- The next m lines describe the handoffs. Each line contains two integers u and v, indicating a directed handoff from runner u to runner v.

## Output Format
- Return single integer: the number of race sequences modulo 10^9+7.

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
