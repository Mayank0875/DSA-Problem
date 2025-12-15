## Title
Urban Park Walk

## Slug
urban-park-walk

## Difficulty
Medium

## Description
A jogger runs exactly k path segments between statues. Each segment is a certain distance.

You need to find a path from Entrance (index 1) to Fountain (index n) that consists of **exactly** `k` segments.
Each segment connects a source statue to a destination statue and has a specific distance associated with it.

Your goal is to calculate the minimum total distance required to travel from Entrance to Fountain using exactly `k` segments. If it is impossible to reach the destination with exactly `k` segments, return -1.

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
We need a path from Entrance to Fountain using exactly 8 segments.
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
There is only one segment from 1 to 2. It is impossible to make 100 segments because once you reach node 2, there are no outgoing segments to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of statues, segments, and the required number of jumps.
- The next `m` lines describe the segments. Each line contains three integers `u`, `v`, and `w`: a segment from `u` to `v` with distance `w`.

## Output Format
- Return one integer: the minimum total distance. If no such path exists, return -1.

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
