## Title
Matter vs Antimatter

## Slug
matter-vs-antimatter

## Difficulty
Medium

## Description
Scientists track particles in a collider. Matter particles follow Magnetic Lines. Antimatter particles follow Void Channels, which exist between nodes not linked by magnets.

The collider has n detectors numbered from 1 to n.
The Magnetic Field connects specific pairs of detectors with direct magnetic lines.
The Void Field is constructed based on a unique rule:
A direct void channel exists between two detectors if and only if there is no magnetic line connecting them.

Moving between any two connected detectors takes exactly 1 hour on either network.
Two particles, The Matter Particle and The Antimatter Particle, depart from detector 1 at the same time, heading for detector n.

1. The Matter Particle travels only using Magnetic Field.
2. The Antimatter Particle travels only using Void Field.

To ensure safety, they must never arrive at the same detector at the same time (except for the final detector n).
Your task is to compute the minimum number of hours required for **both** particles to reach detector n — specifically, the time when the slower particle arrives.
If either particle cannot reach detector n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second particle cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of detectors and the number of magnetic lines.
- The next m lines each contain two integers u and v, representing a magnetic line between detectors u and v.
- The graph is bidirectional. There is at most one magnetic line between any pair of detectors.

## Output Format
- Return a single integer representing the minimum hours required for the last particle to arrive. If it is impossible, return -1.

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
