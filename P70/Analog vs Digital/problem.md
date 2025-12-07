## Title
Analog vs Digital

## Slug
analog-vs-digital

## Difficulty
Medium

## Description
An Analog signal uses Copper Wires. A Digital signal uses Fiber Optics. Fiber connects hubs that Copper doesn't.

The network has n hubs numbered from 1 to n.
The Copper Net connects specific pairs of hubs with direct wires.
The Fiber Net is constructed based on a unique rule:
A direct optic cable exists between two hubs if and only if there is no wire connecting them.

Moving between any two connected hubs takes exactly 1 hour on either network.
Two signals, Analog Signal and Digital Signal, depart from hub 1 at the same time, heading for hub n.

1. Analog Signal travels only using Copper Net.
2. Digital Signal travels only using Fiber Net.

To ensure safety, they must never arrive at the same hub at the same time (except for the final hub n).
Your task is to compute the minimum number of hours required for **both** signals to reach hub n — specifically, the time when the slower signal arrives.
If either signal cannot reach hub n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second signal cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of hubs and the number of wires.
- The next m lines each contain two integers u and v, representing a wire between hubs u and v.
- The graph is bidirectional. There is at most one wire between any pair of hubs.

## Output Format
- Return a single integer representing the minimum hours required for the last signal to arrive. If it is impossible, return -1.

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
