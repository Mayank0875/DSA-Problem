## Title
Train Cargo Shunting

## Slug
train-cargo-shunting

## Difficulty
Medium

## Description
A cargo car is shunted exactly k times between tracks in a yard. Each shunt takes minutes.

You need to find a path from Arrival Track (index 1) to Departure Track (index n) that consists of **exactly** `k` shunts.
Each shunt connects a source track to a destination track and has a specific minutes associated with it.

Your goal is to calculate the minimum total minutes required to travel from Arrival Track to Departure Track using exactly `k` shunts. If it is impossible to reach the destination with exactly `k` shunts, return -1.

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
We need a path from Arrival Track to Departure Track using exactly 8 shunts.
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
There is only one shunt from 1 to 2. It is impossible to make 100 shunts because once you reach node 2, there are no outgoing shunts to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of tracks, shunts, and the required number of jumps.
- The next `m` lines describe the shunts. Each line contains three integers `u`, `v`, and `w`: a shunt from `u` to `v` with minutes `w`.

## Output Format
- Return one integer: the minimum total minutes. If no such path exists, return -1.

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
