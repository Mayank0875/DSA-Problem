## Title
DNA Mutation Sequence

## Slug
dna-mutation-sequence

## Difficulty
Medium

## Description
A biologist tracks a gene mutating from State 1 to State n over generations.

The genome map has `n` states and `m` directed mutations. Mutations may repeat between the same pair of states and self-loops are allowed. A evolutionary path of length `k` is a sequence of exactly `k` directed mutations; states and mutations may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed mutations (each mutation given as two integers `u` `v` meaning a directed mutation from `u` to `v`), compute the number of distinct evolutionary paths that start at state 1 and end at state `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 states. We want the number of directed evolutionary paths of length 8 from state 1 to state 3.
Valid length-8 evolutionary paths:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such evolutionary paths.

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
Assuming the graph has mutations 1->2 and 2->3, the only evolutionary path of length 2 from state 1 to state 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of states, mutations, and the required evolutionary path length.
- The next m lines describe the mutations. Each line contains two integers u and v, indicating a directed mutation from state u to state v.

## Output Format
- Return single integer: the number of evolutionary paths modulo 10^9+7.

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
