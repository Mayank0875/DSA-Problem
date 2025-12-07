## Title
Biological Ancestry Index

## Slug
biological-ancestry-index

## Difficulty
Medium

## Description
Biologists are studying an evolutionary tree of n species. They analyze common ancestors for groups of k species.

Dr. Darwin defines the "Ancestral Diversity" of the structure rooted at a specific species `r` as follows:
Consider every possible set of `k` distinct species from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the species in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique species obtained as LCAs from these sets.
3. The Ancestral Diversity of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Phylogenetic Sum" is defined as the sum of the Ancestral Diversity values for all possible roots `r` from 1 to `n`:
Phylogenetic Sum = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Phylogenetic Sum of the given phylogenetic tree.

Notes:
1. A phylogenetic tree is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted phylogenetic tree is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Phylogenetic Sum is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Phylogenetic Sum is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of species and the size of the sets to consider.
- The following `n-1` lines describe the phylogenetic tree. Each line contains two integers `u` and `v`, indicating a connection between species `u` and `v`.

## Output Format
- Return one integer: the Phylogenetic Sum.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
