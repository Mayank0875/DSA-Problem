## Title
Glacier Expedition Steps

## Slug
glacier-expedition-steps

## Difficulty
Medium

## Description
Explorers must take exactly k legs between camps to acclimatize. Each leg requires supplies.

You need to find a path from Base Camp (index 1) to Summit (index n) that consists of **exactly** `k` legs.
Each leg connects a source camp to a destination camp and has a specific supplies associated with it.

Your goal is to calculate the minimum total supplies required to travel from Base Camp to Summit using exactly `k` legs. If it is impossible to reach the destination with exactly `k` legs, return -1.

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
We need a path from Base Camp to Summit using exactly 8 legs.
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
There is only one leg from 1 to 2. It is impossible to make 100 legs because once you reach node 2, there are no outgoing legs to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of camps, legs, and the required number of jumps.
- The next `m` lines describe the legs. Each line contains three integers `u`, `v`, and `w`: a leg from `u` to `v` with supplies `w`.

## Output Format
- Return one integer: the minimum total supplies. If no such path exists, return -1.

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
