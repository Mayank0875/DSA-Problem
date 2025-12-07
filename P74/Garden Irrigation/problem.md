## Title
Garden Irrigation

## Slug
garden-irrigation

## Difficulty
Medium

## Description
Sprinklers are connected by pipes. The gardener sets up zones where two adjacent sprinklers run together. Each sprinkler belongs to one zone.

The structure is a tree with n sprinklers and n-1 pipes.
A zone is formed between two sprinklers connected by a pipe.
However, each sprinkler can be part of at most one zone.

Your task is to calculate the maximum number of zones that can be formed.

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
One optimal set of zones is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 zones.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form zones (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of sprinklers.
- The next n-1 lines each contain two integers u and v, representing a pipe between sprinkler u and sprinkler v.

## Output Format
- Return a single integer representing the maximum number of zones.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
