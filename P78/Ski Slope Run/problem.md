## Title
Ski Slope Run

## Slug
ski-slope-run

## Difficulty
Medium

## Description
A skier takes exactly k lifts and runs to reach the bottom lodge. Each run has a difficulty rating.

You need to find a path from Peak (index 1) to Lodge (index n) that consists of **exactly** `k` runs.
Each run connects a source lift station to a destination lift station and has a specific difficulty associated with it.

Your goal is to calculate the minimum total difficulty required to travel from Peak to Lodge using exactly `k` runs. If it is impossible to reach the destination with exactly `k` runs, return -1.

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
We need a path from Peak to Lodge using exactly 8 runs.
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
There is only one run from 1 to 2. It is impossible to make 100 runs because once you reach node 2, there are no outgoing runs to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of stations, runs, and the required number of jumps.
- The next `m` lines describe the runs. Each line contains three integers `u`, `v`, and `w`: a run from `u` to `v` with difficulty `w`.

## Output Format
- Return one integer: the minimum total difficulty. If no such path exists, return -1.

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
