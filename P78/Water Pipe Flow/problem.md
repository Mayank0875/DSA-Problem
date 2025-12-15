## Title
Water Pipe Flow

## Slug
water-pipe-flow

## Difficulty
Medium

## Description
Water flows through exactly k pipe segments to reach a tank. Each segment causes pressure loss.

You need to find a path from Source Pump (index 1) to Tank (index n) that consists of **exactly** `k` flows.
Each flow connects a source junction to a destination junction and has a specific pressure loss associated with it.

Your goal is to calculate the minimum total pressure loss required to travel from Source Pump to Tank using exactly `k` flows. If it is impossible to reach the destination with exactly `k` flows, return -1.

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
We need a path from Source Pump to Tank using exactly 8 flows.
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
There is only one flow from 1 to 2. It is impossible to make 100 flows because once you reach node 2, there are no outgoing flows to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of junctions, flows, and the required number of jumps.
- The next `m` lines describe the flows. Each line contains three integers `u`, `v`, and `w`: a flow from `u` to `v` with pressure loss `w`.

## Output Format
- Return one integer: the minimum total pressure loss. If no such path exists, return -1.

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
