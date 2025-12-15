## Title
Electric Grid Load

## Slug
electric-grid-load

## Difficulty
Medium

## Description
Power is routed through exactly k substations to balance the load. Transmission loses voltage.

You need to find a path from Power Plant (index 1) to City Grid (index n) that consists of **exactly** `k` transmissions.
Each transmission connects a source substation to a destination substation and has a specific voltage loss associated with it.

Your goal is to calculate the minimum total voltage loss required to travel from Power Plant to City Grid using exactly `k` transmissions. If it is impossible to reach the destination with exactly `k` transmissions, return -1.

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
We need a path from Power Plant to City Grid using exactly 8 transmissions.
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
There is only one transmission from 1 to 2. It is impossible to make 100 transmissions because once you reach node 2, there are no outgoing transmissions to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of substations, transmissions, and the required number of jumps.
- The next `m` lines describe the transmissions. Each line contains three integers `u`, `v`, and `w`: a transmission from `u` to `v` with voltage loss `w`.

## Output Format
- Return one integer: the minimum total voltage loss. If no such path exists, return -1.

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
