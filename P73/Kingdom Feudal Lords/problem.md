## Title
Kingdom Feudal Lords

## Slug
kingdom-feudal-lords

## Difficulty
Medium

## Description
A kingdom has n fiefdoms. The King analyzes which lords govern common territories for groups of k vassals.

The King defines the "Feudal Authority" of the structure rooted at a specific fiefdom `r` as follows:
Consider every possible set of `k` distinct fiefdoms from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the fiefdoms in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique fiefdoms obtained as LCAs from these sets.
3. The Feudal Authority of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Political Stability" is defined as the sum of the Feudal Authority values for all possible roots `r` from 1 to `n`:
Political Stability = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Political Stability of the given kingdom map.

Notes:
1. A kingdom map is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted kingdom map is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Political Stability is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Political Stability is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of fiefdoms and the size of the sets to consider.
- The following `n-1` lines describe the kingdom map. Each line contains two integers `u` and `v`, indicating a connection between fiefdoms `u` and `v`.

## Output Format
- Return one integer: the Political Stability.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
