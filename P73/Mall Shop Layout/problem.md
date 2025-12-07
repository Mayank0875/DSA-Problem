## Title
Mall Shop Layout

## Slug
mall-shop-layout

## Difficulty
Medium

## Description
A mall has n shops. The architect identifies corridors leading to k stores.

The Architect defines the "Foot Traffic" of the structure rooted at a specific shop `r` as follows:
Consider every possible set of `k` distinct shops from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the shops in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique shops obtained as LCAs from these sets.
3. The Foot Traffic of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Mall Flow" is defined as the sum of the Foot Traffic values for all possible roots `r` from 1 to `n`:
Mall Flow = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Mall Flow of the given floor plan.

Notes:
1. A floor plan is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted floor plan is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Mall Flow is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Mall Flow is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of shops and the size of the sets to consider.
- The following `n-1` lines describe the floor plan. Each line contains two integers `u` and `v`, indicating a connection between shops `u` and `v`.

## Output Format
- Return one integer: the Mall Flow.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
