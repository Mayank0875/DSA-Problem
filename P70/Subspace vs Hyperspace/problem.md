## Title
Subspace vs Hyperspace

## Slug
subspace-vs-hyperspace

## Difficulty
Medium

## Description
Fleet A uses Subspace. Fleet B uses Hyperspace. Hyperspace links stars not connected by Subspace frequencies.

The sector has n stars numbered from 1 to n.
The Subspace connects specific pairs of stars with direct channels.
The Hyperspace is constructed based on a unique rule:
A direct jump exists between two stars if and only if there is no channel connecting them.

Moving between any two connected stars takes exactly 1 hour on either network.
Two fleets, Fleet A and Fleet B, depart from star 1 at the same time, heading for star n.

1. Fleet A travels only using Subspace.
2. Fleet B travels only using Hyperspace.

To ensure safety, they must never arrive at the same star at the same time (except for the final star n).
Your task is to compute the minimum number of hours required for **both** fleets to reach star n — specifically, the time when the slower fleet arrives.
If either fleet cannot reach star n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second fleet cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of stars and the number of channels.
- The next m lines each contain two integers u and v, representing a channel between stars u and v.
- The graph is bidirectional. There is at most one channel between any pair of stars.

## Output Format
- Return a single integer representing the minimum hours required for the last fleet to arrive. If it is impossible, return -1.

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
