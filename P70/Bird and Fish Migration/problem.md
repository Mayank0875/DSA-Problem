## Title
Bird and Fish Migration

## Slug
bird-and-fish-migration

## Difficulty
Medium

## Description
A Bird and a Fish migrate from Point 1 to Point n. The Bird uses Air Currents, while the Fish uses River Currents. Rivers flow between points only if there is no Air Current.

The ecosystem has n habitats numbered from 1 to n.
The Air Stream connects specific pairs of habitats with direct air currents.
The River Stream is constructed based on a unique rule:
A direct river current exists between two habitats if and only if there is no air current connecting them.

Moving between any two connected habitats takes exactly 1 hour on either network.
Two animals, The Bird and The Fish, depart from habitat 1 at the same time, heading for habitat n.

1. The Bird travels only using Air Stream.
2. The Fish travels only using River Stream.

To ensure safety, they must never arrive at the same habitat at the same time (except for the final habitat n).
Your task is to compute the minimum number of hours required for **both** animals to reach habitat n — specifically, the time when the slower animal arrives.
If either animal cannot reach habitat n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second animal cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of habitats and the number of air currents.
- The next m lines each contain two integers u and v, representing a air current between habitats u and v.
- The graph is bidirectional. There is at most one air current between any pair of habitats.

## Output Format
- Return a single integer representing the minimum hours required for the last animal to arrive. If it is impossible, return -1.

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
