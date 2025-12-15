## Title
Chess Knight Training

## Slug
chess-knight-training

## Difficulty
Medium

## Description
A chess knight must make exactly k moves to reach a target square. Each move accumulates 'fatigue' points based on the distance type.

You need to find a path from Start Square (index 1) to Target Square (index n) that consists of **exactly** `k` moves.
Each move connects a source square to a destination square and has a specific fatigue associated with it.

Your goal is to calculate the minimum total fatigue required to travel from Start Square to Target Square using exactly `k` moves. If it is impossible to reach the destination with exactly `k` moves, return -1.

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
We need a path from Start Square to Target Square using exactly 8 moves.
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
There is only one move from 1 to 2. It is impossible to make 100 moves because once you reach node 2, there are no outgoing moves to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of squares, moves, and the required number of jumps.
- The next `m` lines describe the moves. Each line contains three integers `u`, `v`, and `w`: a move from `u` to `v` with fatigue `w`.

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
