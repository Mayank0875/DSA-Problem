## Title
Chemical Reaction Path

## Slug
chemical-reaction-path

## Difficulty
Medium

## Description
A synthesis has n compounds. Chemists find intermediates common to k products.

The Chemist defines the "Intermediate Utility" of the structure rooted at a specific compound `r` as follows:
Consider every possible set of `k` distinct compounds from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the compounds in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique compounds obtained as LCAs from these sets.
3. The Intermediate Utility of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Synthesis Versatility" is defined as the sum of the Intermediate Utility values for all possible roots `r` from 1 to `n`:
Synthesis Versatility = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Synthesis Versatility of the given reaction pathway.

Notes:
1. A reaction pathway is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted reaction pathway is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Synthesis Versatility is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Synthesis Versatility is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of compounds and the size of the sets to consider.
- The following `n-1` lines describe the reaction pathway. Each line contains two integers `u` and `v`, indicating a connection between compounds `u` and `v`.

## Output Format
- Return one integer: the Synthesis Versatility.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
