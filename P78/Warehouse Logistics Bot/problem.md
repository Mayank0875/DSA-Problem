## Title
Warehouse Logistics Bot

## Slug
warehouse-logistics-bot

## Difficulty
Medium

## Description
A bot moves packages. It must make exactly k movements between shelves to calibrate its sensors before docking. Each move uses battery.

You need to find a path from Pickup Zone (index 1) to Docking Bay (index n) that consists of **exactly** `k` movements.
Each movement connects a source shelf to a destination shelf and has a specific battery associated with it.

Your goal is to calculate the minimum total battery required to travel from Pickup Zone to Docking Bay using exactly `k` movements. If it is impossible to reach the destination with exactly `k` movements, return -1.

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
We need a path from Pickup Zone to Docking Bay using exactly 8 movements.
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
There is only one movement from 1 to 2. It is impossible to make 100 movements because once you reach node 2, there are no outgoing movements to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of shelves, movements, and the required number of jumps.
- The next `m` lines describe the movements. Each line contains three integers `u`, `v`, and `w`: a movement from `u` to `v` with battery `w`.

## Output Format
- Return one integer: the minimum total battery. If no such path exists, return -1.

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
