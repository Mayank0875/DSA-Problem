## Title
Server Redundancy

## Slug
server-redundancy

## Difficulty
Medium

## Description
Servers in a data center are wired in a tree. To ensure redundancy, servers are paired up for active-passive failover. Each server can only belong to one failover pair.

The structure is a tree with n servers and n-1 cables.
A failover pair is formed between two servers connected by a cable.
However, each server can be part of at most one failover pair.

Your task is to calculate the maximum number of failover pairs that can be formed.

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
One optimal set of failover pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 failover pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form failover pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of servers.
- The next n-1 lines each contain two integers u and v, representing a cable between server u and server v.

## Output Format
- Return a single integer representing the maximum number of failover pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
