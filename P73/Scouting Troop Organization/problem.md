## Title
Scouting Troop Organization

## Slug
scouting-troop-organization

## Difficulty
Medium

## Description
A troop has n scouts. Leaders find patrol leaders guiding k scouts.

The Leader defines the "Leadership Reach" of the structure rooted at a specific scout `r` as follows:
Consider every possible set of `k` distinct scouts from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the scouts in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique scouts obtained as LCAs from these sets.
3. The Leadership Reach of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Troop Cohesion" is defined as the sum of the Leadership Reach values for all possible roots `r` from 1 to `n`:
Troop Cohesion = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Troop Cohesion of the given troop hierarchy.

Notes:
1. A troop hierarchy is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted troop hierarchy is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Troop Cohesion is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Troop Cohesion is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of scouts and the size of the sets to consider.
- The following `n-1` lines describe the troop hierarchy. Each line contains two integers `u` and `v`, indicating a connection between scouts `u` and `v`.

## Output Format
- Return one integer: the Troop Cohesion.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
