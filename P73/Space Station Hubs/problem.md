## Title
Space Station Hubs

## Slug
space-station-hubs

## Difficulty
Medium

## Description
A station has n modules. The architect calculates which modules act as hubs connecting groups of k other modules.

The Architect defines the "Hub Capacity" of the structure rooted at a specific module `r` as follows:
Consider every possible set of `k` distinct modules from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the modules in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique modules obtained as LCAs from these sets.
3. The Hub Capacity of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Station Design Score" is defined as the sum of the Hub Capacity values for all possible roots `r` from 1 to `n`:
Station Design Score = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Station Design Score of the given module layout.

Notes:
1. A module layout is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted module layout is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Station Design Score is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Station Design Score is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of modules and the size of the sets to consider.
- The following `n-1` lines describe the module layout. Each line contains two integers `u` and `v`, indicating a connection between modules `u` and `v`.

## Output Format
- Return one integer: the Station Design Score.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
