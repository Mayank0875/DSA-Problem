## Title
Ant Colony Tunnels

## Slug
ant-colony-tunnels

## Difficulty
Medium

## Description
An ant colony has n chambers. Biologists study which chambers serve as junctions for k foraging ants.

The Researcher defines the "Junction Traffic" of the structure rooted at a specific chamber `r` as follows:
Consider every possible set of `k` distinct chambers from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the chambers in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique chambers obtained as LCAs from these sets.
3. The Junction Traffic of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Colony Flow" is defined as the sum of the Junction Traffic values for all possible roots `r` from 1 to `n`:
Colony Flow = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Colony Flow of the given tunnel system.

Notes:
1. A tunnel system is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted tunnel system is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Colony Flow is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Colony Flow is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of chambers and the size of the sets to consider.
- The following `n-1` lines describe the tunnel system. Each line contains two integers `u` and `v`, indicating a connection between chambers `u` and `v`.

## Output Format
- Return one integer: the Colony Flow.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
