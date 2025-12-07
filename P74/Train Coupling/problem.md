## Title
Train Coupling

## Slug
train-coupling

## Difficulty
Medium

## Description
Train carriages are on a switching yard track structure (tree). The yard master wants to couple adjacent carriages into pairs for moving. Each carriage can be coupled once.

The structure is a tree with n carriages and n-1 couplers.
A coupled set is formed between two carriages connected by a coupler.
However, each carriage can be part of at most one coupled set.

Your task is to calculate the maximum number of coupled sets that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of coupled sets is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 coupled sets.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form coupled sets (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of carriages.
- The next n-1 lines each contain two integers u and v, representing a coupler between carriage u and carriage v.

## Output Format
- Return a single integer representing the maximum number of coupled sets.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
