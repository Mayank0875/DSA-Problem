## Title
Decision Making Process

## Slug
decision-making-process

## Difficulty
Medium

## Description
A decision model has n steps. Analysts determine the pivotal decisions that lead to sets of k outcomes.

The Analyst defines the "Pivot Importance" of the structure rooted at a specific step `r` as follows:
Consider every possible set of `k` distinct steps from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the steps in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique steps obtained as LCAs from these sets.
3. The Pivot Importance of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Process Clarity" is defined as the sum of the Pivot Importance values for all possible roots `r` from 1 to `n`:
Process Clarity = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Process Clarity of the given decision tree.

Notes:
1. A decision tree is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted decision tree is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Process Clarity is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Process Clarity is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of steps and the size of the sets to consider.
- The following `n-1` lines describe the decision tree. Each line contains two integers `u` and `v`, indicating a connection between steps `u` and `v`.

## Output Format
- Return one integer: the Process Clarity.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
