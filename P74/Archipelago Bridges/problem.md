## Title
Archipelago Bridges

## Slug
archipelago-bridges

## Difficulty
Medium

## Description
Islands are connected by bridges. The government wants to designate pairs of sister islands. Each island can be a sister to only one neighbor.

The structure is a tree with n islands and n-1 bridges.
A sister pair is formed between two islands connected by a bridge.
However, each island can be part of at most one sister pair.

Your task is to calculate the maximum number of sister pairs that can be formed.

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
One optimal set of sister pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 sister pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form sister pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of islands.
- The next n-1 lines each contain two integers u and v, representing a bridge between island u and island v.

## Output Format
- Return a single integer representing the maximum number of sister pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
