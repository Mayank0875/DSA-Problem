## Title
Hospital Department Flow

## Slug
hospital-department-flow

## Difficulty
Medium

## Description
A hospital has n departments. Administrators analyze which departments coordinate care for groups of k patients.

The Administrator defines the "Care Coordination" of the structure rooted at a specific department `r` as follows:
Consider every possible set of `k` distinct departments from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the departments in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique departments obtained as LCAs from these sets.
3. The Care Coordination of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Hospital Efficiency" is defined as the sum of the Care Coordination values for all possible roots `r` from 1 to `n`:
Hospital Efficiency = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Hospital Efficiency of the given department chart.

Notes:
1. A department chart is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted department chart is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Hospital Efficiency is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Hospital Efficiency is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of departments and the size of the sets to consider.
- The following `n-1` lines describe the department chart. Each line contains two integers `u` and `v`, indicating a connection between departments `u` and `v`.

## Output Format
- Return one integer: the Hospital Efficiency.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
