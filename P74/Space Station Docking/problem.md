## Title
Space Station Docking

## Slug
space-station-docking

## Difficulty
Medium

## Description
Modules of a space station are connected via airlocks. During an emergency, modules must seal off in pairs to preserve oxygen. Each module can only seal with one neighbor.

The structure is a tree with n modules and n-1 airlocks.
A sealed pair is formed between two modules connected by a airlock.
However, each module can be part of at most one sealed pair.

Your task is to calculate the maximum number of sealed pairs that can be formed.

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
One optimal set of sealed pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 sealed pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form sealed pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of modules.
- The next n-1 lines each contain two integers u and v, representing a airlock between module u and module v.

## Output Format
- Return a single integer representing the maximum number of sealed pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
