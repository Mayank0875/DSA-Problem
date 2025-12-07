## Title
Telescope Data Array

## Slug
telescope-data-array

## Difficulty
Medium

## Description
An array has n sensors. Scientists identify data aggregators for groups of k sensors.

The Scientist defines the "Data Aggregation" of the structure rooted at a specific sensor `r` as follows:
Consider every possible set of `k` distinct sensors from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the sensors in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique sensors obtained as LCAs from these sets.
3. The Data Aggregation of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Array Sensitivity" is defined as the sum of the Data Aggregation values for all possible roots `r` from 1 to `n`:
Array Sensitivity = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Array Sensitivity of the given sensor array.

Notes:
1. A sensor array is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted sensor array is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Array Sensitivity is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Array Sensitivity is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of sensors and the size of the sets to consider.
- The following `n-1` lines describe the sensor array. Each line contains two integers `u` and `v`, indicating a connection between sensors `u` and `v`.

## Output Format
- Return one integer: the Array Sensitivity.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
