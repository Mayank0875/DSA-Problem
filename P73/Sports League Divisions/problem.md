## Title
Sports League Divisions

## Slug
sports-league-divisions

## Difficulty
Medium

## Description
A league has n teams. The Commissioner looks at how divisions are formed by groups of k teams.

The Commissioner defines the "Division Weight" of the structure rooted at a specific team `r` as follows:
Consider every possible set of `k` distinct teams from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the teams in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique teams obtained as LCAs from these sets.
3. The Division Weight of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "League Structure Value" is defined as the sum of the Division Weight values for all possible roots `r` from 1 to `n`:
League Structure Value = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the League Structure Value of the given league hierarchy.

Notes:
1. A league hierarchy is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted league hierarchy is the deepest node that is an ancestor of all nodes in the set.

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
The calculated League Structure Value is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated League Structure Value is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of teams and the size of the sets to consider.
- The following `n-1` lines describe the league hierarchy. Each line contains two integers `u` and `v`, indicating a connection between teams `u` and `v`.

## Output Format
- Return one integer: the League Structure Value.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
