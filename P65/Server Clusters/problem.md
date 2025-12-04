## Title
Server Clusters

## Slug
server-clusters

## Difficulty
Medium

## Description
A data center has N servers connected by one-way data pipes. A Cluster is a group of servers that can all ping each other successfully.

Two servers a and b belong to the same Cluster if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of data pipes.
In other words, two servers are in the same Cluster if they are mutually reachable.

Your task is to: Determine how many Clusters exist in total.

## Examples

### 1

#### Input
5 6
1 2
2 3
3 1
3 4
4 5
5 4

#### Output
2

#### Explanation
The servers form two distinct groups where round-trip traversal is possible within each group.
Servers {1, 2, 3} form one Cluster.
Path: 1 -> 2 -> 3 -> 1.
Servers {4, 5} form another Cluster.
Path: 4 -> 5 -> 4.
Total Clusters: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 servers and 1 one-way pipe.
Pipe: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Clusters.

## Input Format
- The first line contains two integers n and m: the number of servers and data pipes.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way pipe from server a to server b.

## Output Format
- Return one integer: the total number of Clusters.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search
