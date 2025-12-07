## Title
River Confluence Analysis

## Slug
river-confluence-analysis

## Difficulty
Medium

## Description
Hydrologists map n points along a river system. They study how k tributaries converge at specific points depending on the source.

The Hydrologist defines the "Confluence Factor" of the structure rooted at a specific point `r` as follows:
Consider every possible set of `k` distinct points from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the points in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique points obtained as LCAs from these sets.
3. The Confluence Factor of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Basin Complexity" is defined as the sum of the Confluence Factor values for all possible roots `r` from 1 to `n`:
Basin Complexity = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Basin Complexity of the given river system.

Notes:
1. A river system is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted river system is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Basin Complexity is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Basin Complexity is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of points and the size of the sets to consider.
- The following `n-1` lines describe the river system. Each line contains two integers `u` and `v`, indicating a connection between points `u` and `v`.

## Output Format
- Return one integer: the Basin Complexity.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
