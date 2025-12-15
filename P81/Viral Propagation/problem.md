## Title
Viral Propagation

## Slug
viral-propagation

## Difficulty
Medium

## Description
A digital virus is spreading from the Patient Zero server (node 1) to the Mainframe (node n).

The network has `n` servers and `m` directed connections. Connections may repeat between the same pair of servers and self-loops are allowed. A infection chain of length `k` is a sequence of exactly `k` directed connections; servers and connections may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed connections (each connection given as two integers `u` `v` meaning a directed connection from `u` to `v`), compute the number of distinct infection chains that start at server 1 and end at server `n` with length exactly `k`. Output the answer modulo 1000000007.

## Examples

### 1

#### Input
3 4 8
1 2
2 3
3 1
3 2

#### Output
2

#### Explanation
We have 3 servers. We want the number of directed infection chains of length 8 from server 1 to server 3.
Valid length-8 infection chains:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such infection chains.

### 2

#### Input
3 4 2
1 2
2 3
3 1
3 2

#### Output
1

#### Explanation
Assuming the graph has connections 1->2 and 2->3, the only infection chain of length 2 from server 1 to server 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of servers, connections, and the required infection chain length.
- The next m lines describe the connections. Each line contains two integers u and v, indicating a directed connection from server u to server v.

## Output Format
- Return single integer: the number of infection chains modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ 10^5
- 1 ≤ k ≤ 10^18
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
