## Title
Political Hierarchy

## Slug
political-hierarchy

## Difficulty
Medium

## Description
A government has n officials. Analysts check which officials oversee k departments.

The Analyst defines the "Oversight Reach" of the structure rooted at a specific official `r` as follows:
Consider every possible set of `k` distinct officials from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the officials in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique officials obtained as LCAs from these sets.
3. The Oversight Reach of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Bureaucracy Score" is defined as the sum of the Oversight Reach values for all possible roots `r` from 1 to `n`:
Bureaucracy Score = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Bureaucracy Score of the given org chart.

Notes:
1. A org chart is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted org chart is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Bureaucracy Score is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Bureaucracy Score is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of officials and the size of the sets to consider.
- The following `n-1` lines describe the org chart. Each line contains two integers `u` and `v`, indicating a connection between officials `u` and `v`.

## Output Format
- Return one integer: the Bureaucracy Score.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
