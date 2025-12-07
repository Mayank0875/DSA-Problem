## Title
Distributed Computing

## Slug
distributed-computing

## Difficulty
Medium

## Description
Compute nodes are linked in a tree. The system scheduler pairs adjacent nodes to perform parallel processing tasks. Each node handles one task.

The structure is a tree with n nodes and n-1 links.
A processing pair is formed between two nodes connected by a link.
However, each node can be part of at most one processing pair.

Your task is to calculate the maximum number of processing pairs that can be formed.

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
One optimal set of processing pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 processing pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form processing pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of nodes.
- The next n-1 lines each contain two integers u and v, representing a link between node u and node v.

## Output Format
- Return a single integer representing the maximum number of processing pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
