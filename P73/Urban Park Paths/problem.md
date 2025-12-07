## Title
Urban Park Paths

## Slug
urban-park-paths

## Difficulty
Medium

## Description
A park has n landmarks. Landscapers find junctions connecting k scenic spots.

The Landscaper defines the "Path Utility" of the structure rooted at a specific landmark `r` as follows:
Consider every possible set of `k` distinct landmarks from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the landmarks in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique landmarks obtained as LCAs from these sets.
3. The Path Utility of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Park Layout Score" is defined as the sum of the Path Utility values for all possible roots `r` from 1 to `n`:
Park Layout Score = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Park Layout Score of the given path network.

Notes:
1. A path network is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted path network is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Park Layout Score is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Park Layout Score is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of landmarks and the size of the sets to consider.
- The following `n-1` lines describe the path network. Each line contains two integers `u` and `v`, indicating a connection between landmarks `u` and `v`.

## Output Format
- Return one integer: the Park Layout Score.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
