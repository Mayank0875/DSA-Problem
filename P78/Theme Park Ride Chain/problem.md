## Title
Theme Park Ride Chain

## Slug
theme-park-ride-chain

## Difficulty
Medium

## Description
A visitor rides exactly k rides in sequence. Walking between rides is tiring.

You need to find a path from Entrance (index 1) to Exit (index n) that consists of **exactly** `k` walks.
Each walk connects a source ride to a destination ride and has a specific fatigue associated with it.

Your goal is to calculate the minimum total fatigue required to travel from Entrance to Exit using exactly `k` walks. If it is impossible to reach the destination with exactly `k` walks, return -1.

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
We need a path from Entrance to Exit using exactly 8 walks.
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
There is only one walk from 1 to 2. It is impossible to make 100 walks because once you reach node 2, there are no outgoing walks to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of rides, walks, and the required number of jumps.
- The next `m` lines describe the walks. Each line contains three integers `u`, `v`, and `w`: a walk from `u` to `v` with fatigue `w`.

## Output Format
- Return one integer: the minimum total fatigue. If no such path exists, return -1.

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
