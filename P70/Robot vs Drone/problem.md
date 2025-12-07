## Title
Robot vs Drone

## Slug
robot-vs-drone

## Difficulty
Medium

## Description
A Ground Robot uses walkways. An Aerial Drone uses flight paths. Flight paths are allowed between buildings only if there is no walkway.

The campus has n buildings numbered from 1 to n.
The Ground Net connects specific pairs of buildings with direct walkways.
The Sky Net is constructed based on a unique rule:
A direct flight path exists between two buildings if and only if there is no walkway connecting them.

Moving between any two connected buildings takes exactly 1 hour on either network.
Two machines, The Robot and The Drone, depart from building 1 at the same time, heading for building n.

1. The Robot travels only using Ground Net.
2. The Drone travels only using Sky Net.

To ensure safety, they must never arrive at the same building at the same time (except for the final building n).
Your task is to compute the minimum number of hours required for **both** machines to reach building n — specifically, the time when the slower machine arrives.
If either machine cannot reach building n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second machine cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of buildings and the number of walkways.
- The next m lines each contain two integers u and v, representing a walkway between buildings u and v.
- The graph is bidirectional. There is at most one walkway between any pair of buildings.

## Output Format
- Return a single integer representing the minimum hours required for the last machine to arrive. If it is impossible, return -1.

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
