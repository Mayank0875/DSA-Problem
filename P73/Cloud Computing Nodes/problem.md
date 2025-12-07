## Title
Cloud Computing Nodes

## Slug
cloud-computing-nodes

## Difficulty
Medium

## Description
A cloud has n compute nodes. Architects find balancers managing k instances.

The Architect defines the "Load Balance" of the structure rooted at a specific node `r` as follows:
Consider every possible set of `k` distinct nodes from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the nodes in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique nodes obtained as LCAs from these sets.
3. The Load Balance of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Cloud Efficiency" is defined as the sum of the Load Balance values for all possible roots `r` from 1 to `n`:
Cloud Efficiency = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Cloud Efficiency of the given compute cluster.

Notes:
1. A compute cluster is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted compute cluster is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Cloud Efficiency is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Cloud Efficiency is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of nodes and the size of the sets to consider.
- The following `n-1` lines describe the compute cluster. Each line contains two integers `u` and `v`, indicating a connection between nodes `u` and `v`.

## Output Format
- Return one integer: the Cloud Efficiency.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
