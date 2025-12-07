## Title
Security Guard Patrols

## Slug
security-guard-patrols

## Difficulty
Medium

## Description
A facility has checkpoints connected by corridors in a tree layout. Guards patrol in pairs. A pair is assigned to a specific corridor connecting two checkpoints. Each checkpoint can only be managed by one patrol pair.

The structure is a tree with n checkpoints and n-1 corridors.
A patrol assignment is formed between two checkpoints connected by a corridor.
However, each checkpoint can be part of at most one patrol assignment.

Your task is to calculate the maximum number of patrol assignments that can be formed.

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
One optimal set of patrol assignments is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 patrol assignments.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form patrol assignments (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of checkpoints.
- The next n-1 lines each contain two integers u and v, representing a corridor between checkpoint u and checkpoint v.

## Output Format
- Return a single integer representing the maximum number of patrol assignments.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
