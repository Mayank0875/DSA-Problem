## Title
Submarine Sonar Ping

## Slug
submarine-sonar-ping

## Difficulty
Medium

## Description
A sonar ping bounces exactly k times between underwater canyons to reach a sub. Signal degrades with distance.

You need to find a path from Source (index 1) to Submarine (index n) that consists of **exactly** `k` bounces.
Each bounce connects a source canyon wall to a destination canyon wall and has a specific degradation associated with it.

Your goal is to calculate the minimum total degradation required to travel from Source to Submarine using exactly `k` bounces. If it is impossible to reach the destination with exactly `k` bounces, return -1.

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
We need a path from Source to Submarine using exactly 8 bounces.
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
There is only one bounce from 1 to 2. It is impossible to make 100 bounces because once you reach node 2, there are no outgoing bounces to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of walls, bounces, and the required number of jumps.
- The next `m` lines describe the bounces. Each line contains three integers `u`, `v`, and `w`: a bounce from `u` to `v` with degradation `w`.

## Output Format
- Return one integer: the minimum total degradation. If no such path exists, return -1.

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
