## Title
Chemical Reaction

## Slug
chemical-reaction

## Difficulty
Medium

## Description
A molecule transforms from Reactant (node 1) to Product (node n).

The reaction vessel has `n` compounds and `m` directed reactions. Reactions may repeat between the same pair of compounds and self-loops are allowed. A synthesis path of length `k` is a sequence of exactly `k` directed reactions; compounds and reactions may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed reactions (each reaction given as two integers `u` `v` meaning a directed reaction from `u` to `v`), compute the number of distinct synthesis paths that start at compound 1 and end at compound `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 compounds. We want the number of directed synthesis paths of length 8 from compound 1 to compound 3.
Valid length-8 synthesis paths:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such synthesis paths.

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
Assuming the graph has reactions 1->2 and 2->3, the only synthesis path of length 2 from compound 1 to compound 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of compounds, reactions, and the required synthesis path length.
- The next m lines describe the reactions. Each line contains two integers u and v, indicating a directed reaction from compound u to compound v.

## Output Format
- Return single integer: the number of synthesis paths modulo 10^9+7.

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
