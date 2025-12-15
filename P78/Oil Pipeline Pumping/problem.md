## Title
Oil Pipeline Pumping

## Slug
oil-pipeline-pumping

## Difficulty
Medium

## Description
Oil is pumped through exactly k stations. Each pumping stage requires electricity.

You need to find a path from Well (index 1) to Refinery (index n) that consists of **exactly** `k` pumps.
Each pump connects a source station to a destination station and has a specific electricity associated with it.

Your goal is to calculate the minimum total electricity required to travel from Well to Refinery using exactly `k` pumps. If it is impossible to reach the destination with exactly `k` pumps, return -1.

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
We need a path from Well to Refinery using exactly 8 pumps.
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
There is only one pump from 1 to 2. It is impossible to make 100 pumps because once you reach node 2, there are no outgoing pumps to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of stations, pumps, and the required number of jumps.
- The next `m` lines describe the pumps. Each line contains three integers `u`, `v`, and `w`: a pump from `u` to `v` with electricity `w`.

## Output Format
- Return one integer: the minimum total electricity. If no such path exists, return -1.

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
