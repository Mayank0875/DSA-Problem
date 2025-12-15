## Title
Satellite Orbit Transfer

## Slug
satellite-orbit-transfer

## Difficulty
Medium

## Description
A satellite makes exactly k orbital maneuvers to change altitude. Each maneuver uses fuel.

You need to find a path from Low Orbit (index 1) to Geo Orbit (index n) that consists of **exactly** `k` maneuvers.
Each maneuver connects a source position to a destination position and has a specific fuel associated with it.

Your goal is to calculate the minimum total fuel required to travel from Low Orbit to Geo Orbit using exactly `k` maneuvers. If it is impossible to reach the destination with exactly `k` maneuvers, return -1.

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
We need a path from Low Orbit to Geo Orbit using exactly 8 maneuvers.
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
There is only one maneuver from 1 to 2. It is impossible to make 100 maneuvers because once you reach node 2, there are no outgoing maneuvers to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of positions, maneuvers, and the required number of jumps.
- The next `m` lines describe the maneuvers. Each line contains three integers `u`, `v`, and `w`: a maneuver from `u` to `v` with fuel `w`.

## Output Format
- Return one integer: the minimum total fuel. If no such path exists, return -1.

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
