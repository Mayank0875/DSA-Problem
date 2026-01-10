## Title
Oil Pipeline

## Slug
oil-pipeline

## Difficulty
Medium

## Description
Crude oil is pumped from wells. All flow must reach the Refinery.

There are $n$ pumps numbered from $1$ to $n$, connected by $n-1$ pipes. The network forms a tree structure (there is exactly one path between any two pumps). Currently, all pipes are one-way.

Production requires flow to the **Refinery (Node 1)**. To ensure success, every other pump must be able to reach Refinery by traveling along the pipes in the correct direction.

You are given the current orientation of the pipes. Your task is to determine the **minimum** number of pipes that need to be reversed so that every pump can reach Refinery.

## Examples

### 1

#### Input
6
1 2
2 4
3 2
5 1
5 6

#### Output
3

#### Explanation
The destination is Refinery (1).
- Pipe 1->2 points away from 1. Needs reversal.
- Pipe 2->4 points away from 1. Needs reversal.
- Pipe 3->2 points towards 2 (and effectively towards 1). OK.
- Pipe 5->1 points towards 1. OK.
- Pipe 5->6 points away from 1 (via 5). Needs reversal.
Total reversals: 3.

### 2

#### Input
5
2 1
2 3
4 3
4 5

#### Output
2

#### Explanation
Pipes 2->3 and 4->5 need to be reversed.

## Input Format
- The first line contains an integer $n$ — the number of pumps.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way pipe from pump $u$ to pump $v$.

## Output Format
- Return a single integer representing the minimum number of pipes that need to be changed.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ u, v ≤ n
- The graph is guaranteed to be a tree.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
tree, depth-first-search, breadth-first-search, graph

## Company
google, amazon
