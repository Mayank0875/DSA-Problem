## Title
Network Packet Hopping

## Slug
network-packet-hopping

## Difficulty
Medium

## Description
A secure data packet must hop exactly k times through a mesh network to scramble its trace before reaching the destination server.

You need to find a path from Source Server (index 1) to Target Server (index n) that consists of **exactly** `k` hops.
Each hop connects a source server to a destination server and has a specific latency associated with it.

Your goal is to calculate the minimum total latency required to travel from Source Server to Target Server using exactly `k` hops. If it is impossible to reach the destination with exactly `k` hops, return -1.

## Examples

### 1

#### Input
3 4 8
1 2 5
2 3 4
3 1 1
3 2 2

#### Output
27

#### Explanation
We need a path from Source Server to Target Server using exactly 8 hops.
Consider the path: 1 -> 2 -> 3 -> 2 -> 3 -> 2 -> 3 -> 2 -> 3.
Costs: 5 + 4 + 2 + 4 + 2 + 4 + 2 + 4 = 27.
This is the minimum cost possible.

### 2

#### Input
2 1 100
1 2 10

#### Output
-1

#### Explanation
There is only one hop from 1 to 2. It is impossible to make 100 hops because once you reach node 2, there are no outgoing hops to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of servers, hops, and the required number of jumps.
- The next `m` lines describe the hops. Each line contains three integers `u`, `v`, and `w`: a hop from `u` to `v` with latency `w`.

## Output Format
- Return one integer: the minimum total latency. If no such path exists, return -1.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ n * (n - 1)
- 1 ≤ k ≤ 10^9
- 1 ≤ u, v ≤ n
- 1 ≤ w ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
