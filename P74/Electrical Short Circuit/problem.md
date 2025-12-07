## Title
Electrical Short Circuit

## Slug
electrical-short-circuit

## Difficulty
Medium

## Description
A circuit grid is a tree of nodes. A flaw causes adjacent nodes to short-circuit in pairs. Each node can only participate in one short.

The structure is a tree with n nodes and n-1 wires.
A short is formed between two nodes connected by a wire.
However, each node can be part of at most one short.

Your task is to calculate the maximum number of shorts that can be formed.

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
One optimal set of shorts is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 shorts.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form shorts (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of nodes.
- The next n-1 lines each contain two integers u and v, representing a wire between node u and node v.

## Output Format
- Return a single integer representing the maximum number of shorts.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
