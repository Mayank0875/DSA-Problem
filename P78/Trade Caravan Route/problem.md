## Title
Trade Caravan Route

## Slug
trade-caravan-route

## Difficulty
Medium

## Description
A caravan must stop at exactly k trading posts to maximize market exposure before reaching the capital. Travel between posts costs gold.

You need to find a path from Border Post (index 1) to Capital Post (index n) that consists of **exactly** `k` journeys.
Each journey connects a source post to a destination post and has a specific gold associated with it.

Your goal is to calculate the minimum total gold required to travel from Border Post to Capital Post using exactly `k` journeys. If it is impossible to reach the destination with exactly `k` journeys, return -1.

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
We need a path from Border Post to Capital Post using exactly 8 journeys.
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
There is only one journey from 1 to 2. It is impossible to make 100 journeys because once you reach node 2, there are no outgoing journeys to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of posts, journeys, and the required number of jumps.
- The next `m` lines describe the journeys. Each line contains three integers `u`, `v`, and `w`: a journey from `u` to `v` with gold `w`.

## Output Format
- Return one integer: the minimum total gold. If no such path exists, return -1.

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
