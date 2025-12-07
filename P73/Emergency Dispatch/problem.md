## Title
Emergency Dispatch

## Slug
emergency-dispatch

## Difficulty
Medium

## Description
A city has n districts. The chief finds central stations covering k incidents.

The Chief defines the "Response Coverage" of the structure rooted at a specific district `r` as follows:
Consider every possible set of `k` distinct districts from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the districts in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique districts obtained as LCAs from these sets.
3. The Response Coverage of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "City Safety Score" is defined as the sum of the Response Coverage values for all possible roots `r` from 1 to `n`:
City Safety Score = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the City Safety Score of the given district map.

Notes:
1. A district map is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted district map is the deepest node that is an ancestor of all nodes in the set.

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
The calculated City Safety Score is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated City Safety Score is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of districts and the size of the sets to consider.
- The following `n-1` lines describe the district map. Each line contains two integers `u` and `v`, indicating a connection between districts `u` and `v`.

## Output Format
- Return one integer: the City Safety Score.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
