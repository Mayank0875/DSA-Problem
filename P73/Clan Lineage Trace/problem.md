## Title
Clan Lineage Trace

## Slug
clan-lineage-trace

## Difficulty
Medium

## Description
A historical clan has n recorded ancestors. Historians trace the lineage heads for groups of k descendants.

The Historian defines the "Lineage Strength" of the structure rooted at a specific person `r` as follows:
Consider every possible set of `k` distinct people from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the people in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique people obtained as LCAs from these sets.
3. The Lineage Strength of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Clan Heritage Value" is defined as the sum of the Lineage Strength values for all possible roots `r` from 1 to `n`:
Clan Heritage Value = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Clan Heritage Value of the given lineage tree.

Notes:
1. A lineage tree is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted lineage tree is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Clan Heritage Value is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Clan Heritage Value is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of people and the size of the sets to consider.
- The following `n-1` lines describe the lineage tree. Each line contains two integers `u` and `v`, indicating a connection between people `u` and `v`.

## Output Format
- Return one integer: the Clan Heritage Value.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
