## Title
Magic vs Tech Duel

## Slug
magic-vs-tech-duel

## Difficulty
Medium

## Description
A Mage and a Cyborg race to the Crystal Tower. The Mage uses Teleportation Gates, while the Cyborg uses Tech Bridges. Tech Bridges are built only where Teleportation Gates do not exist.

The realm has n sectors numbered from 1 to n.
The Teleport Network connects specific pairs of sectors with direct gates.
The Tech Network is constructed based on a unique rule:
A direct bridge exists between two sectors if and only if there is no gate connecting them.

Moving between any two connected sectors takes exactly 1 hour on either network.
Two competitors, The Mage and The Cyborg, depart from sector 1 at the same time, heading for sector n.

1. The Mage travels only using Teleport Network.
2. The Cyborg travels only using Tech Network.

To ensure safety, they must never arrive at the same sector at the same time (except for the final sector n).
Your task is to compute the minimum number of hours required for **both** competitors to reach sector n — specifically, the time when the slower competitor arrives.
If either competitor cannot reach sector n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second competitor cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of sectors and the number of gates.
- The next m lines each contain two integers u and v, representing a gate between sectors u and v.
- The graph is bidirectional. There is at most one gate between any pair of sectors.

## Output Format
- Return a single integer representing the minimum hours required for the last competitor to arrive. If it is impossible, return -1.

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
