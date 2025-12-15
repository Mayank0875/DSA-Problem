## Title
Dungeon Crawler Levels

## Slug
dungeon-crawler-levels

## Difficulty
Medium

## Description
A hero clears exactly k floors to reach the boss. Clearing a floor takes health points.

You need to find a path from Lobby (index 1) to Boss Floor (index n) that consists of **exactly** `k` clears.
Each clear connects a source floor to a destination floor and has a specific health associated with it.

Your goal is to calculate the minimum total health required to travel from Lobby to Boss Floor using exactly `k` clears. If it is impossible to reach the destination with exactly `k` clears, return -1.

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
We need a path from Lobby to Boss Floor using exactly 8 clears.
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
There is only one clear from 1 to 2. It is impossible to make 100 clears because once you reach node 2, there are no outgoing clears to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of floors, clears, and the required number of jumps.
- The next `m` lines describe the clears. Each line contains three integers `u`, `v`, and `w`: a clear from `u` to `v` with health `w`.

## Output Format
- Return one integer: the minimum total health. If no such path exists, return -1.

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
