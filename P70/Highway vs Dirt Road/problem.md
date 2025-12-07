## Title
Highway vs Dirt Road

## Slug
highway-vs-dirt-road

## Difficulty
Medium

## Description
A Sports Car races a Rally Car. The Sports Car uses Paved Highways. The Rally Car uses Dirt Tracks, existing where Highways don't.

The county has n towns numbered from 1 to n.
The Paved Net connects specific pairs of towns with direct highways.
The Offroad Net is constructed based on a unique rule:
A direct dirt track exists between two towns if and only if there is no highway connecting them.

Moving between any two connected towns takes exactly 1 hour on either network.
Two cars, The Sports Car and The Rally Car, depart from town 1 at the same time, heading for town n.

1. The Sports Car travels only using Paved Net.
2. The Rally Car travels only using Offroad Net.

To ensure safety, they must never arrive at the same town at the same time (except for the final town n).
Your task is to compute the minimum number of hours required for **both** cars to reach town n — specifically, the time when the slower car arrives.
If either car cannot reach town n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second car cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of towns and the number of highways.
- The next m lines each contain two integers u and v, representing a highway between towns u and v.
- The graph is bidirectional. There is at most one highway between any pair of towns.

## Output Format
- Return a single integer representing the minimum hours required for the last car to arrive. If it is impossible, return -1.

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
