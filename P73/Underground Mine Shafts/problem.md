## Title
Underground Mine Shafts

## Slug
underground-mine-shafts

## Difficulty
Medium

## Description
A mine has n excavation points. The foreman identifies key junctions used by teams of k miners.

The Foreman defines the "Junction Usage" of the structure rooted at a specific point `r` as follows:
Consider every possible set of `k` distinct points from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the points in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique points obtained as LCAs from these sets.
3. The Junction Usage of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Mine Accessibility" is defined as the sum of the Junction Usage values for all possible roots `r` from 1 to `n`:
Mine Accessibility = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Mine Accessibility of the given mine layout.

Notes:
1. A mine layout is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted mine layout is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Mine Accessibility is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Mine Accessibility is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of points and the size of the sets to consider.
- The following `n-1` lines describe the mine layout. Each line contains two integers `u` and `v`, indicating a connection between points `u` and `v`.

## Output Format
- Return one integer: the Mine Accessibility.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
