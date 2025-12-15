## Title
Molecular Bonding Chain

## Slug
molecular-bonding-chain

## Difficulty
Medium

## Description
A synthetic molecule is built by forming a chain of exactly k bonds between atoms. Each bond requires energy to stabilize.

You need to find a path from Start Atom (index 1) to End Atom (index n) that consists of **exactly** `k` bonds.
Each bond connects a source atom to a destination atom and has a specific energy associated with it.

Your goal is to calculate the minimum total energy required to travel from Start Atom to End Atom using exactly `k` bonds. If it is impossible to reach the destination with exactly `k` bonds, return -1.

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
We need a path from Start Atom to End Atom using exactly 8 bonds.
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
There is only one bond from 1 to 2. It is impossible to make 100 bonds because once you reach node 2, there are no outgoing bonds to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of atoms, bonds, and the required number of jumps.
- The next `m` lines describe the bonds. Each line contains three integers `u`, `v`, and `w`: a bond from `u` to `v` with energy `w`.

## Output Format
- Return one integer: the minimum total energy. If no such path exists, return -1.

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
