## Title
Gene Mutation Path

## Slug
gene-mutation-path

## Difficulty
Medium

## Description
A gene sequence mutates exactly k times to evolve into a new variant. Each mutation step has a biological cost.

You need to find a path from Original Gene (index 1) to Variant Gene (index n) that consists of **exactly** `k` mutations.
Each mutation connects a source sequence to a destination sequence and has a specific biological cost associated with it.

Your goal is to calculate the minimum total biological cost required to travel from Original Gene to Variant Gene using exactly `k` mutations. If it is impossible to reach the destination with exactly `k` mutations, return -1.

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
We need a path from Original Gene to Variant Gene using exactly 8 mutations.
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
There is only one mutation from 1 to 2. It is impossible to make 100 mutations because once you reach node 2, there are no outgoing mutations to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of sequences, mutations, and the required number of jumps.
- The next `m` lines describe the mutations. Each line contains three integers `u`, `v`, and `w`: a mutation from `u` to `v` with biological cost `w`.

## Output Format
- Return one integer: the minimum total biological cost. If no such path exists, return -1.

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
