## Title
Solar vs Lunar Power

## Slug
solar-vs-lunar-power

## Difficulty
Medium

## Description
Energy flows through the grid. Solar energy uses Gold Wires. Lunar energy uses Silver Wires. Silver wires connect pylons that Gold wires don't.

The power grid has n pylons numbered from 1 to n.
The Solar Grid connects specific pairs of pylons with direct gold wires.
The Lunar Grid is constructed based on a unique rule:
A direct silver wire exists between two pylons if and only if there is no gold wire connecting them.

Moving between any two connected pylons takes exactly 1 hour on either network.
Two pulses, Solar Pulse and Lunar Pulse, depart from pylon 1 at the same time, heading for pylon n.

1. Solar Pulse travels only using Solar Grid.
2. Lunar Pulse travels only using Lunar Grid.

To ensure safety, they must never arrive at the same pylon at the same time (except for the final pylon n).
Your task is to compute the minimum number of hours required for **both** pulses to reach pylon n — specifically, the time when the slower pulse arrives.
If either pulse cannot reach pylon n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second pulse cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of pylons and the number of gold wires.
- The next m lines each contain two integers u and v, representing a gold wire between pylons u and v.
- The graph is bidirectional. There is at most one gold wire between any pair of pylons.

## Output Format
- Return a single integer representing the minimum hours required for the last pulse to arrive. If it is impossible, return -1.

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
