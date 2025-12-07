## Title
Corporate Hierarchy Score

## Slug
corporate-hierarchy-score

## Difficulty
Medium

## Description
A corporation has n employees arranged in a hierarchy. HR wants to evaluate the robustness of leadership.

The HR Director defines the "Management Relevance" of the structure rooted at a specific employee `r` as follows:
Consider every possible set of `k` distinct employees from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the employees in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique employees obtained as LCAs from these sets.
3. The Management Relevance of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Total Corporate Power" is defined as the sum of the Management Relevance values for all possible roots `r` from 1 to `n`:
Total Corporate Power = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Total Corporate Power of the given hierarchy.

Notes:
1. A hierarchy is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted hierarchy is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Total Corporate Power is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Total Corporate Power is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of employees and the size of the sets to consider.
- The following `n-1` lines describe the hierarchy. Each line contains two integers `u` and `v`, indicating a connection between employees `u` and `v`.

## Output Format
- Return one integer: the Total Corporate Power.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
