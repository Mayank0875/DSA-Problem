## Title
Quantum Leap

## Slug
quantum-leap

## Difficulty
Medium

## Description
A particle jumps from Energy Level 1 to Energy Level n.

The quantum field has `n` levels and `m` directed transitions. Transitions may repeat between the same pair of levels and self-loops are allowed. A trajectory of length `k` is a sequence of exactly `k` directed transitions; levels and transitions may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed transitions (each transition given as two integers `u` `v` meaning a directed transition from `u` to `v`), compute the number of distinct trajectories that start at level 1 and end at level `n` with length exactly `k`. Output the answer modulo 1000000007.

## Examples

### 1

#### Input
3 4 8
1 2
2 3
3 1
3 2

#### Output
2

#### Explanation
We have 3 levels. We want the number of directed trajectories of length 8 from level 1 to level 3.
Valid length-8 trajectories:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such trajectories.

### 2

#### Input
3 4 2
1 2
2 3
3 1
3 2

#### Output
1

#### Explanation
Assuming the graph has transitions 1->2 and 2->3, the only trajectory of length 2 from level 1 to level 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of levels, transitions, and the required trajectory length.
- The next m lines describe the transitions. Each line contains two integers u and v, indicating a directed transition from level u to level v.

## Output Format
- Return single integer: the number of trajectories modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ 10^5
- 1 ≤ k ≤ 10^18
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
