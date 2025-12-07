## Title
Fashion Trend Cycle

## Slug
fashion-trend-cycle

## Difficulty
Medium

## Description
Fashion has n trends. Designers find core styles influencing k modern looks.

The Designer defines the "Style Influence" of the structure rooted at a specific trend `r` as follows:
Consider every possible set of `k` distinct trends from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the trends in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique trends obtained as LCAs from these sets.
3. The Style Influence of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Trend Depth" is defined as the sum of the Style Influence values for all possible roots `r` from 1 to `n`:
Trend Depth = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Trend Depth of the given influence tree.

Notes:
1. A influence tree is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted influence tree is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Trend Depth is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Trend Depth is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of trends and the size of the sets to consider.
- The following `n-1` lines describe the influence tree. Each line contains two integers `u` and `v`, indicating a connection between trends `u` and `v`.

## Output Format
- Return one integer: the Trend Depth.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
