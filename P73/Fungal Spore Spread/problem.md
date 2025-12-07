## Title
Fungal Spore Spread

## Slug
fungal-spore-spread

## Difficulty
Medium

## Description
A fungus has n nodes. Biologists trace the spread from central nodes to k spores.

The Biologist defines the "Spread Potential" of the structure rooted at a specific node `r` as follows:
Consider every possible set of `k` distinct nodes from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the nodes in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique nodes obtained as LCAs from these sets.
3. The Spread Potential of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Mycelium Density" is defined as the sum of the Spread Potential values for all possible roots `r` from 1 to `n`:
Mycelium Density = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Mycelium Density of the given fungal network.

Notes:
1. A fungal network is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted fungal network is the deepest node that is an ancestor of all nodes in the set.

## Examples

### 1

#### Input
6 3
1 2
1 3
2 4
2 5
3 6

#### Output
17

#### Explanation
The calculated Mycelium Density is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Mycelium Density is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of nodes and the size of the sets to consider.
- The following `n-1` lines describe the fungal network. Each line contains two integers `u` and `v`, indicating a connection between nodes `u` and `v`.

## Output Format
- Return one integer: the Mycelium Density.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
