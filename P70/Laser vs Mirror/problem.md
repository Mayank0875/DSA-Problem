## Title
Laser vs Mirror

## Slug
laser-vs-mirror

## Difficulty
Medium

## Description
A Laser beam travels direct paths. A Reflection travels via Mirrors. Mirrors connect points that the direct Laser cannot reach.

The optical table has n components numbered from 1 to n.
The Direct Path connects specific pairs of components with direct beams.
The Reflected Path is constructed based on a unique rule:
A direct reflection exists between two components if and only if there is no beam connecting them.

Moving between any two connected components takes exactly 1 hour on either network.
Two photons, The Laser and The Reflection, depart from component 1 at the same time, heading for component n.

1. The Laser travels only using Direct Path.
2. The Reflection travels only using Reflected Path.

To ensure safety, they must never arrive at the same component at the same time (except for the final component n).
Your task is to compute the minimum number of hours required for **both** photons to reach component n — specifically, the time when the slower photon arrives.
If either photon cannot reach component n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second photon cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of components and the number of beams.
- The next m lines each contain two integers u and v, representing a beam between components u and v.
- The graph is bidirectional. There is at most one beam between any pair of components.

## Output Format
- Return a single integer representing the minimum hours required for the last photon to arrive. If it is impossible, return -1.

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
