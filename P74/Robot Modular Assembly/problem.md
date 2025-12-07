## Title
Robot Modular Assembly

## Slug
robot-modular-assembly

## Difficulty
Medium

## Description
A modular robot is built from units connected in a tree. Engineers want to lock units together in pairs for transport. Each unit can be locked to only one neighbor.

The structure is a tree with n units and n-1 joints.
A locked pair is formed between two units connected by a joint.
However, each unit can be part of at most one locked pair.

Your task is to calculate the maximum number of locked pairs that can be formed.

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
One optimal set of locked pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 locked pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form locked pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of units.
- The next n-1 lines each contain two integers u and v, representing a joint between unit u and unit v.

## Output Format
- Return a single integer representing the maximum number of locked pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
