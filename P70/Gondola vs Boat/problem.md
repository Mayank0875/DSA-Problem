## Title
Gondola vs Boat

## Slug
gondola-vs-boat

## Difficulty
Medium

## Description
In Venice, a Gondola uses Canals. A Pedestrian uses Bridges. Bridges connect islands not linked by a direct Canal route.

The Venice has n islands numbered from 1 to n.
The Waterway connects specific pairs of islands with direct canals.
The Walkway is constructed based on a unique rule:
A direct bridge exists between two islands if and only if there is no canal connecting them.

Moving between any two connected islands takes exactly 1 hour on either network.
Two travelers, The Gondolier and The Pedestrian, depart from island 1 at the same time, heading for island n.

1. The Gondolier travels only using Waterway.
2. The Pedestrian travels only using Walkway.

To ensure safety, they must never arrive at the same island at the same time (except for the final island n).
Your task is to compute the minimum number of hours required for **both** travelers to reach island n — specifically, the time when the slower traveler arrives.
If either traveler cannot reach island n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second traveler cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of islands and the number of canals.
- The next m lines each contain two integers u and v, representing a canal between islands u and v.
- The graph is bidirectional. There is at most one canal between any pair of islands.

## Output Format
- Return a single integer representing the minimum hours required for the last traveler to arrive. If it is impossible, return -1.

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
