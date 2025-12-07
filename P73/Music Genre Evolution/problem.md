## Title
Music Genre Evolution

## Slug
music-genre-evolution

## Difficulty
Medium

## Description
Music history has n genres. Historians find parent genres spawning k sub-genres.

The Historian defines the "Cultural Impact" of the structure rooted at a specific genre `r` as follows:
Consider every possible set of `k` distinct genres from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the genres in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique genres obtained as LCAs from these sets.
3. The Cultural Impact of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Evolution Index" is defined as the sum of the Cultural Impact values for all possible roots `r` from 1 to `n`:
Evolution Index = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Evolution Index of the given genre tree.

Notes:
1. A genre tree is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted genre tree is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Evolution Index is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Evolution Index is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of genres and the size of the sets to consider.
- The following `n-1` lines describe the genre tree. Each line contains two integers `u` and `v`, indicating a connection between genres `u` and `v`.

## Output Format
- Return one integer: the Evolution Index.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
