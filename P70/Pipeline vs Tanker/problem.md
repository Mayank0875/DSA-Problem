## Title
Pipeline vs Tanker

## Slug
pipeline-vs-tanker

## Difficulty
Medium

## Description
Oil flows via Pipelines. Where no Pipeline exists, Tanker Trucks transport it.

The oil field has n depots numbered from 1 to n.
The Pipe Network connects specific pairs of depots with direct pipes.
The Truck Network is constructed based on a unique rule:
A direct truck route exists between two depots if and only if there is no pipe connecting them.

Moving between any two connected depots takes exactly 1 hour on either network.
Two shipments, The Flow and The Truck, depart from depot 1 at the same time, heading for depot n.

1. The Flow travels only using Pipe Network.
2. The Truck travels only using Truck Network.

To ensure safety, they must never arrive at the same depot at the same time (except for the final depot n).
Your task is to compute the minimum number of hours required for **both** shipments to reach depot n — specifically, the time when the slower shipment arrives.
If either shipment cannot reach depot n using their respective network, return -1.

## Examples

### 1

#### Input
4 2
1 3
3 4

#### Output
2

#### Explanation
The smallest possible time is 2. One takes the direct route (1 hour), the other takes a path of length 2.

### 2

#### Input
4 6
1 2
1 3
1 4
2 3
2 4
3 4

#### Output
-1

#### Explanation
The graph is fully connected for one network, meaning the complement network has no edges. The second shipment cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of depots and the number of pipes.
- The next m lines each contain two integers u and v, representing a pipe between depots u and v.
- The graph is bidirectional. There is at most one pipe between any pair of depots.

## Output Format
- Return a single integer representing the minimum hours required for the last shipment to arrive. If it is impossible, return -1.

## Constraints
- 2 ≤ n ≤ 400
- 0 ≤ m ≤ n(n - 1)/2
- 1 ≤ u, v ≤ n
- u ≠ v

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
