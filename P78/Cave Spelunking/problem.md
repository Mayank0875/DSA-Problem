## Title
Cave Spelunking

## Slug
cave-spelunking

## Difficulty
Medium

## Description
A spelunker traverses exactly k tunnels between caverns. Each tunnel is dangerous.

You need to find a path from Entrance (index 1) to Deep Chamber (index n) that consists of **exactly** `k` tunnels.
Each tunnel connects a source cavern to a destination cavern and has a specific danger associated with it.

Your goal is to calculate the minimum total danger required to travel from Entrance to Deep Chamber using exactly `k` tunnels. If it is impossible to reach the destination with exactly `k` tunnels, return -1.

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
We need a path from Entrance to Deep Chamber using exactly 8 tunnels.
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
There is only one tunnel from 1 to 2. It is impossible to make 100 tunnels because once you reach node 2, there are no outgoing tunnels to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of caverns, tunnels, and the required number of jumps.
- The next `m` lines describe the tunnels. Each line contains three integers `u`, `v`, and `w`: a tunnel from `u` to `v` with danger `w`.

## Output Format
- Return one integer: the minimum total danger. If no such path exists, return -1.

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
