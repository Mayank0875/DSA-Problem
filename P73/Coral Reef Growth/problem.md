## Title
Coral Reef Growth

## Slug
coral-reef-growth

## Difficulty
Medium

## Description
A reef has n coral heads. Divers study which bases support k distinct polyps.

The Diver defines the "Support Base" of the structure rooted at a specific head `r` as follows:
Consider every possible set of `k` distinct heads from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the heads in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique heads obtained as LCAs from these sets.
3. The Support Base of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Reef Structure" is defined as the sum of the Support Base values for all possible roots `r` from 1 to `n`:
Reef Structure = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Reef Structure of the given coral formation.

Notes:
1. A coral formation is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted coral formation is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Reef Structure is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Reef Structure is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of heads and the size of the sets to consider.
- The following `n-1` lines describe the coral formation. Each line contains two integers `u` and `v`, indicating a connection between heads `u` and `v`.

## Output Format
- Return one integer: the Reef Structure.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
