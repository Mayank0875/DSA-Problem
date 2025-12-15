## Title
Video Game Quest Chain

## Slug
video-game-quest-chain

## Difficulty
Medium

## Description
A player must complete a chain of exactly k quests. Quests lead from one NPC to another. Each quest takes time to complete.

You need to find a path from First NPC (index 1) to Final Boss (index n) that consists of **exactly** `k` quests.
Each quest connects a source NPC to a destination NPC and has a specific time associated with it.

Your goal is to calculate the minimum total time required to travel from First NPC to Final Boss using exactly `k` quests. If it is impossible to reach the destination with exactly `k` quests, return -1.

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
We need a path from First NPC to Final Boss using exactly 8 quests.
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
There is only one quest from 1 to 2. It is impossible to make 100 quests because once you reach node 2, there are no outgoing quests to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of NPCs, quests, and the required number of jumps.
- The next `m` lines describe the quests. Each line contains three integers `u`, `v`, and `w`: a quest from `u` to `v` with time `w`.

## Output Format
- Return one integer: the minimum total time. If no such path exists, return -1.

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
