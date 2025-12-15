## Title
Spy Flight Route

## Slug
spy-flight-route

## Difficulty
Medium

## Description
A spy plane must fly exactly k legs between airports to avoid pattern detection software. Each flight leg consumes fuel.

You need to find a path from Origin Airport (index 1) to Destination Airport (index n) that consists of **exactly** `k` flights.
Each flight connects a source airport to a destination airport and has a specific fuel associated with it.

Your goal is to calculate the minimum total fuel required to travel from Origin Airport to Destination Airport using exactly `k` flights. If it is impossible to reach the destination with exactly `k` flights, return -1.

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
We need a path from Origin Airport to Destination Airport using exactly 8 flights.
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
There is only one flight from 1 to 2. It is impossible to make 100 flights because once you reach node 2, there are no outgoing flights to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of airports, flights, and the required number of jumps.
- The next `m` lines describe the flights. Each line contains three integers `u`, `v`, and `w`: a flight from `u` to `v` with fuel `w`.

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
