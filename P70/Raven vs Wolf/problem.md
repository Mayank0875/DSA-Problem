## Title
Raven vs Wolf

## Slug
raven-vs-wolf

## Difficulty
Medium

## Description
A Raven flies message. A Wolf runs it. The Wolf runs trails connecting woods not reachable by direct flight.

The wilds has n groves numbered from 1 to n.
The Flight connects specific pairs of groves with direct flights.
The Run is constructed based on a unique rule:
A direct path exists between two groves if and only if there is no flight connecting them.

Moving between any two connected groves takes exactly 1 hour on either network.
Two messengers, The Raven and The Wolf, depart from grove 1 at the same time, heading for grove n.

1. The Raven travels only using Flight.
2. The Wolf travels only using Run.

To ensure safety, they must never arrive at the same grove at the same time (except for the final grove n).
Your task is to compute the minimum number of hours required for **both** messengers to reach grove n — specifically, the time when the slower messenger arrives.
If either messenger cannot reach grove n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second messenger cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of groves and the number of flights.
- The next m lines each contain two integers u and v, representing a flight between groves u and v.
- The graph is bidirectional. There is at most one flight between any pair of groves.

## Output Format
- Return a single integer representing the minimum hours required for the last messenger to arrive. If it is impossible, return -1.

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
