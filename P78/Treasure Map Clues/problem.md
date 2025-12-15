## Title
Treasure Map Clues

## Slug
treasure-map-clues

## Difficulty
Medium

## Description
A pirate follows exactly k clues. Each clue leads from one landmark to another. Travel is tiresome.

You need to find a path from Landing Beach (index 1) to Buried Treasure (index n) that consists of **exactly** `k` travels.
Each travel connects a source landmark to a destination landmark and has a specific effort associated with it.

Your goal is to calculate the minimum total effort required to travel from Landing Beach to Buried Treasure using exactly `k` travels. If it is impossible to reach the destination with exactly `k` travels, return -1.

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
We need a path from Landing Beach to Buried Treasure using exactly 8 travels.
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
There is only one travel from 1 to 2. It is impossible to make 100 travels because once you reach node 2, there are no outgoing travels to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of landmarks, travels, and the required number of jumps.
- The next `m` lines describe the travels. Each line contains three integers `u`, `v`, and `w`: a travel from `u` to `v` with effort `w`.

## Output Format
- Return one integer: the minimum total effort. If no such path exists, return -1.

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
