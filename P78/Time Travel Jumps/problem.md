## Title
Time Travel Jumps

## Slug
time-travel-jumps

## Difficulty
Medium

## Description
A traveler jumps through exactly k timelines to fix a paradox. Each jump requires chronons.

You need to find a path from Original Timeline (index 1) to Fixed Timeline (index n) that consists of **exactly** `k` jumps.
Each jump connects a source timeline to a destination timeline and has a specific chronons associated with it.

Your goal is to calculate the minimum total chronons required to travel from Original Timeline to Fixed Timeline using exactly `k` jumps. If it is impossible to reach the destination with exactly `k` jumps, return -1.

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
We need a path from Original Timeline to Fixed Timeline using exactly 8 jumps.
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
There is only one jump from 1 to 2. It is impossible to make 100 jumps because once you reach node 2, there are no outgoing jumps to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of timelines, jumps, and the required number of jumps.
- The next `m` lines describe the jumps. Each line contains three integers `u`, `v`, and `w`: a jump from `u` to `v` with chronons `w`.

## Output Format
- Return one integer: the minimum total chronons. If no such path exists, return -1.

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
