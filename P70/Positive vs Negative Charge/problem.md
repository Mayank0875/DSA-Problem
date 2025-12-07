## Title
Positive vs Negative Charge

## Slug
positive-vs-negative-charge

## Difficulty
Medium

## Description
Electrons move along Conductive Wires. Ions move along Electrolytic Channels. Channels exist where wires are absent.

The circuit has n nodes numbered from 1 to n.
The Wire Grid connects specific pairs of nodes with direct wires.
The Ion Grid is constructed based on a unique rule:
A direct channel exists between two nodes if and only if there is no wire connecting them.

Moving between any two connected nodes takes exactly 1 hour on either network.
Two charges, The Electron and The Ion, depart from node 1 at the same time, heading for node n.

1. The Electron travels only using Wire Grid.
2. The Ion travels only using Ion Grid.

To ensure safety, they must never arrive at the same node at the same time (except for the final node n).
Your task is to compute the minimum number of hours required for **both** charges to reach node n — specifically, the time when the slower charge arrives.
If either charge cannot reach node n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second charge cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of nodes and the number of wires.
- The next m lines each contain two integers u and v, representing a wire between nodes u and v.
- The graph is bidirectional. There is at most one wire between any pair of nodes.

## Output Format
- Return a single integer representing the minimum hours required for the last charge to arrive. If it is impossible, return -1.

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
