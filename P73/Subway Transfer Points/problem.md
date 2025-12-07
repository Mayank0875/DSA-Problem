## Title
Subway Transfer Points

## Slug
subway-transfer-points

## Difficulty
Medium

## Description
A subway has n stations. Planners analyze transfer stations connecting k stops.

The Planner defines the "Transfer Volume" of the structure rooted at a specific station `r` as follows:
Consider every possible set of `k` distinct stations from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the stations in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique stations obtained as LCAs from these sets.
3. The Transfer Volume of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Transit Efficiency" is defined as the sum of the Transfer Volume values for all possible roots `r` from 1 to `n`:
Transit Efficiency = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Transit Efficiency of the given metro map.

Notes:
1. A metro map is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted metro map is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Transit Efficiency is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Transit Efficiency is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of stations and the size of the sets to consider.
- The following `n-1` lines describe the metro map. Each line contains two integers `u` and `v`, indicating a connection between stations `u` and `v`.

## Output Format
- Return one integer: the Transit Efficiency.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
