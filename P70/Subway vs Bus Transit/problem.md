## Title
Subway vs Bus Transit

## Slug
subway-vs-bus-transit

## Difficulty
Medium

## Description
Commuters race across the city. One takes the Subway, the other takes the Bus. Bus routes cover connections that the Subway does not serve.

The metro system has n stations numbered from 1 to n.
The Subway Line connects specific pairs of stations with direct tracks.
The Bus Line is constructed based on a unique rule:
A direct route exists between two stations if and only if there is no track connecting them.

Moving between any two connected stations takes exactly 1 hour on either network.
Two commuters, The Subway Rider and The Bus Rider, depart from station 1 at the same time, heading for station n.

1. The Subway Rider travels only using Subway Line.
2. The Bus Rider travels only using Bus Line.

To ensure safety, they must never arrive at the same station at the same time (except for the final station n).
Your task is to compute the minimum number of hours required for **both** commuters to reach station n — specifically, the time when the slower commuter arrives.
If either commuter cannot reach station n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second commuter cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of stations and the number of tracks.
- The next m lines each contain two integers u and v, representing a track between stations u and v.
- The graph is bidirectional. There is at most one track between any pair of stations.

## Output Format
- Return a single integer representing the minimum hours required for the last commuter to arrive. If it is impossible, return -1.

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
