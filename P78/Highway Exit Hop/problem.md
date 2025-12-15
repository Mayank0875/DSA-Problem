## Title
Highway Exit Hop

## Slug
highway-exit-hop

## Difficulty
Medium

## Description
A driver takes exactly k highway segments between exits. Tolls are collected on each segment.

You need to find a path from On-Ramp (index 1) to Off-Ramp (index n) that consists of **exactly** `k` segments.
Each segment connects a source exit to a destination exit and has a specific toll associated with it.

Your goal is to calculate the minimum total toll required to travel from On-Ramp to Off-Ramp using exactly `k` segments. If it is impossible to reach the destination with exactly `k` segments, return -1.

## Examples

### 1

#### Input
3 4 8
1 2 5
2 3 4
3 1 1
3 2 2

#### Output
27

#### Explanation
We need a path from On-Ramp to Off-Ramp using exactly 8 segments.
Consider the path: 1 -> 2 -> 3 -> 2 -> 3 -> 2 -> 3 -> 2 -> 3.
Costs: 5 + 4 + 2 + 4 + 2 + 4 + 2 + 4 = 27.
This is the minimum cost possible.

### 2

#### Input
2 1 100
1 2 10

#### Output
-1

#### Explanation
There is only one segment from 1 to 2. It is impossible to make 100 segments because once you reach node 2, there are no outgoing segments to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of exits, segments, and the required number of jumps.
- The next `m` lines describe the segments. Each line contains three integers `u`, `v`, and `w`: a segment from `u` to `v` with toll `w`.

## Output Format
- Return one integer: the minimum total toll. If no such path exists, return -1.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ n * (n - 1)
- 1 ≤ k ≤ 10^9
- 1 ≤ u, v ≤ n
- 1 ≤ w ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
