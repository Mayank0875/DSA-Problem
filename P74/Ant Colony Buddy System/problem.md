## Title
Ant Colony Buddy System

## Slug
ant-colony-buddy-system

## Difficulty
Medium

## Description
Ant chambers are connected by tunnels. For a dangerous foraging expedition, ants from adjacent chambers pair up. Each chamber provides one ant, and they pair with a neighbor.

The structure is a tree with n chambers and n-1 tunnels.
A foraging pair is formed between two chambers connected by a tunnel.
However, each chamber can be part of at most one foraging pair.

Your task is to calculate the maximum number of foraging pairs that can be formed.

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
One optimal set of foraging pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 foraging pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form foraging pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of chambers.
- The next n-1 lines each contain two integers u and v, representing a tunnel between chamber u and chamber v.

## Output Format
- Return a single integer representing the maximum number of foraging pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
