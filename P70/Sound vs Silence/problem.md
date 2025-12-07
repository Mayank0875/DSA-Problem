## Title
Sound vs Silence

## Slug
sound-vs-silence

## Difficulty
Medium

## Description
A Sound Wave and a Silence Pulse move through an acoustic chamber. Sound travels through Resonators. Silence travels through Dampeners, which connect nodes without Resonators.

The chamber has n points numbered from 1 to n.
The Resonance Grid connects specific pairs of points with direct resonators.
The Damping Grid is constructed based on a unique rule:
A direct dampener exists between two points if and only if there is no resonator connecting them.

Moving between any two connected points takes exactly 1 hour on either network.
Two waves, The Sound Wave and The Silence Pulse, depart from point 1 at the same time, heading for point n.

1. The Sound Wave travels only using Resonance Grid.
2. The Silence Pulse travels only using Damping Grid.

To ensure safety, they must never arrive at the same point at the same time (except for the final point n).
Your task is to compute the minimum number of hours required for **both** waves to reach point n — specifically, the time when the slower wave arrives.
If either wave cannot reach point n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second wave cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of points and the number of resonators.
- The next m lines each contain two integers u and v, representing a resonator between points u and v.
- The graph is bidirectional. There is at most one resonator between any pair of points.

## Output Format
- Return a single integer representing the minimum hours required for the last wave to arrive. If it is impossible, return -1.

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
