## Title
Magical Ritual Steps

## Slug
magical-ritual-steps

## Difficulty
Medium

## Description
A wizard performs a ritual requiring exactly k incantations. Each incantation transitions the magic state from one rune to another, consuming mana.

You need to find a path from Base Rune (index 1) to Final Rune (index n) that consists of **exactly** `k` incantations.
Each incantation connects a source rune to a destination rune and has a specific mana associated with it.

Your goal is to calculate the minimum total mana required to travel from Base Rune to Final Rune using exactly `k` incantations. If it is impossible to reach the destination with exactly `k` incantations, return -1.

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
We need a path from Base Rune to Final Rune using exactly 8 incantations.
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
There is only one incantation from 1 to 2. It is impossible to make 100 incantations because once you reach node 2, there are no outgoing incantations to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of runes, incantations, and the required number of jumps.
- The next `m` lines describe the incantations. Each line contains three integers `u`, `v`, and `w`: a incantation from `u` to `v` with mana `w`.

## Output Format
- Return one integer: the minimum total mana. If no such path exists, return -1.

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
