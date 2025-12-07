## Title
Train vs Plane Race

## Slug
train-vs-plane-race

## Difficulty
Medium

## Description
Two travelers are racing from City 1 to City n. One uses the High-Speed Rail network, and the other uses the Flight network. Flights exist between cities only if there is no direct rail line.

The transport system has n cities numbered from 1 to n.
The Rail Network connects specific pairs of cities with direct tracks.
The Flight Network is constructed based on a unique rule:
A direct flight path exists between two cities if and only if there is no track connecting them.

Moving between any two connected cities takes exactly 1 hour on either network.
Two travelers, The Train Passenger and The Air Passenger, depart from city 1 at the same time, heading for city n.

1. The Train Passenger travels only using Rail Network.
2. The Air Passenger travels only using Flight Network.

To ensure safety, they must never arrive at the same city at the same time (except for the final city n).
Your task is to compute the minimum number of hours required for **both** travelers to reach city n — specifically, the time when the slower traveler arrives.
If either traveler cannot reach city n using their respective network, return -1.

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
- The first line contains two integers n and m, representing the number of cities and the number of tracks.
- The next m lines each contain two integers u and v, representing a track between cities u and v.
- The graph is bidirectional. There is at most one track between any pair of cities.

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
