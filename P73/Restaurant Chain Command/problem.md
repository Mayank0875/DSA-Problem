## Title
Restaurant Chain Command

## Slug
restaurant-chain-command

## Difficulty
Medium

## Description
A chain has n locations. The CEO checks regional managers covering k sites.

The CEO defines the "Regional Control" of the structure rooted at a specific location `r` as follows:
Consider every possible set of `k` distinct locations from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the locations in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique locations obtained as LCAs from these sets.
3. The Regional Control of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Chain Command Score" is defined as the sum of the Regional Control values for all possible roots `r` from 1 to `n`:
Chain Command Score = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Chain Command Score of the given chain hierarchy.

Notes:
1. A chain hierarchy is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted chain hierarchy is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Chain Command Score is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Chain Command Score is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of locations and the size of the sets to consider.
- The following `n-1` lines describe the chain hierarchy. Each line contains two integers `u` and `v`, indicating a connection between locations `u` and `v`.

## Output Format
- Return one integer: the Chain Command Score.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
