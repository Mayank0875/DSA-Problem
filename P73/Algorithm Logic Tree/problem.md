## Title
Algorithm Logic Tree

## Slug
algorithm-logic-tree

## Difficulty
Medium

## Description
An algorithm has n states. Computer scientists find states leading to k outputs.

The Scientist defines the "State Criticality" of the structure rooted at a specific state `r` as follows:
Consider every possible set of `k` distinct states from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the states in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique states obtained as LCAs from these sets.
3. The State Criticality of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Logic Depth" is defined as the sum of the State Criticality values for all possible roots `r` from 1 to `n`:
Logic Depth = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Logic Depth of the given state machine.

Notes:
1. A state machine is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted state machine is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Logic Depth is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Logic Depth is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of states and the size of the sets to consider.
- The following `n-1` lines describe the state machine. Each line contains two integers `u` and `v`, indicating a connection between states `u` and `v`.

## Output Format
- Return one integer: the Logic Depth.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
