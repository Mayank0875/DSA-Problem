## Title
Chemical Reaction Sequence

## Slug
chemical-reaction-sequence

## Difficulty
Medium

## Description
A reaction must undergo exactly k intermediate transformations to reach a stable state. Each step releases heat.

You need to find a path from Reactant (index 1) to Product (index n) that consists of **exactly** `k` reactions.
Each reaction connects a source state to a destination state and has a specific heat associated with it.

Your goal is to calculate the minimum total heat required to travel from Reactant to Product using exactly `k` reactions. If it is impossible to reach the destination with exactly `k` reactions, return -1.

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
We need a path from Reactant to Product using exactly 8 reactions.
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
There is only one reaction from 1 to 2. It is impossible to make 100 reactions because once you reach node 2, there are no outgoing reactions to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of states, reactions, and the required number of jumps.
- The next `m` lines describe the reactions. Each line contains three integers `u`, `v`, and `w`: a reaction from `u` to `v` with heat `w`.

## Output Format
- Return one integer: the minimum total heat. If no such path exists, return -1.

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
