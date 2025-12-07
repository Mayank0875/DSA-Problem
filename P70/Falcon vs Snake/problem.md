## Title
Falcon vs Snake

## Slug
falcon-vs-snake

## Difficulty
Medium

## Description
A Falcon flies between peaks. A Snake slithers through valleys. Valleys connect peaks not linked by a direct flight path.

The canyon has n peaks numbered from 1 to n.
The Sky Way connects specific pairs of peaks with direct flights.
The Ground Way is constructed based on a unique rule:
A direct slither exists between two peaks if and only if there is no flight connecting them.

Moving between any two connected peaks takes exactly 1 hour on either network.
Two predators, The Falcon and The Snake, depart from peak 1 at the same time, heading for peak n.

1. The Falcon travels only using Sky Way.
2. The Snake travels only using Ground Way.

To ensure safety, they must never arrive at the same peak at the same time (except for the final peak n).
Your task is to compute the minimum number of hours required for **both** predators to reach peak n — specifically, the time when the slower predator arrives.
If either predator cannot reach peak n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second predator cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of peaks and the number of flights.
- The next m lines each contain two integers u and v, representing a flight between peaks u and v.
- The graph is bidirectional. There is at most one flight between any pair of peaks.

## Output Format
- Return a single integer representing the minimum hours required for the last predator to arrive. If it is impossible, return -1.

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
