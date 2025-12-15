## Title
Space Station Patrol

## Slug
space-station-patrol

## Difficulty
Medium

## Description
A security drone patrols a station. It must visit exactly k sectors in sequence ending at the charging bay. Travel consumes power.

You need to find a path from Hangar (index 1) to Charging Bay (index n) that consists of **exactly** `k` travels.
Each travel connects a source sector to a destination sector and has a specific power associated with it.

Your goal is to calculate the minimum total power required to travel from Hangar to Charging Bay using exactly `k` travels. If it is impossible to reach the destination with exactly `k` travels, return -1.

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
We need a path from Hangar to Charging Bay using exactly 8 travels.
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
- The first line contains three integers `n`, `m`, and `k`: the number of sectors, travels, and the required number of jumps.
- The next `m` lines describe the travels. Each line contains three integers `u`, `v`, and `w`: a travel from `u` to `v` with power `w`.

## Output Format
- Return one integer: the minimum total power. If no such path exists, return -1.

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
