## Title
Radio vs Fiber Optic

## Slug
radio-vs-fiber-optic

## Difficulty
Medium

## Description
Data packets are sent via Radio Towers and Fiber Cables. Fiber Cables connect nodes that do not have a direct Radio link.

The comm grid has n nodes numbered from 1 to n.
The Radio Grid connects specific pairs of nodes with direct radio links.
The Fiber Grid is constructed based on a unique rule:
A direct fiber cable exists between two nodes if and only if there is no radio link connecting them.

Moving between any two connected nodes takes exactly 1 hour on either network.
Two packets, Packet A and Packet B, depart from node 1 at the same time, heading for node n.

1. Packet A travels only using Radio Grid.
2. Packet B travels only using Fiber Grid.

To ensure safety, they must never arrive at the same node at the same time (except for the final node n).
Your task is to compute the minimum number of hours required for **both** packets to reach node n — specifically, the time when the slower packet arrives.
If either packet cannot reach node n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second packet cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of nodes and the number of radio links.
- The next m lines each contain two integers u and v, representing a radio link between nodes u and v.
- The graph is bidirectional. There is at most one radio link between any pair of nodes.

## Output Format
- Return a single integer representing the minimum hours required for the last packet to arrive. If it is impossible, return -1.

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
