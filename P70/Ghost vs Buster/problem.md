## Title
Ghost vs Buster

## Slug
ghost-vs-buster

## Difficulty
Medium

## Description
A Ghost phases through walls. A Buster uses doors. Doors connect rooms that aren't linked by a ghost-permeable wall.

The mansion has n rooms numbered from 1 to n.
The Phase Path connects specific pairs of rooms with direct phases.
The Door Path is constructed based on a unique rule:
A direct doorway exists between two rooms if and only if there is no phase connecting them.

Moving between any two connected rooms takes exactly 1 hour on either network.
Two entities, The Ghost and The Buster, depart from room 1 at the same time, heading for room n.

1. The Ghost travels only using Phase Path.
2. The Buster travels only using Door Path.

To ensure safety, they must never arrive at the same room at the same time (except for the final room n).
Your task is to compute the minimum number of hours required for **both** entities to reach room n — specifically, the time when the slower entity arrives.
If either entity cannot reach room n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second entity cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of rooms and the number of phases.
- The next m lines each contain two integers u and v, representing a phase between rooms u and v.
- The graph is bidirectional. There is at most one phase between any pair of rooms.

## Output Format
- Return a single integer representing the minimum hours required for the last entity to arrive. If it is impossible, return -1.

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
