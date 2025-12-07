## Title
Express Elevator vs Service Stairs

## Slug
express-elevator-vs-service-stairs

## Difficulty
Medium

## Description
The CEO takes the Express Elevator. The Janitor takes Service Stairs. Stairs connect floors the elevator skips.

The HQ has n levels numbered from 1 to n.
The Elevator Shaft connects specific pairs of levels with direct stops.
The Stairwell is constructed based on a unique rule:
A direct climb exists between two levels if and only if there is no stop connecting them.

Moving between any two connected levels takes exactly 1 hour on either network.
Two staff, The CEO and The Janitor, depart from level 1 at the same time, heading for level n.

1. The CEO travels only using Elevator Shaft.
2. The Janitor travels only using Stairwell.

To ensure safety, they must never arrive at the same level at the same time (except for the final level n).
Your task is to compute the minimum number of hours required for **both** staff to reach level n — specifically, the time when the slower staff member arrives.
If either staff member cannot reach level n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second staff member cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of levels and the number of stops.
- The next m lines each contain two integers u and v, representing a stop between levels u and v.
- The graph is bidirectional. There is at most one stop between any pair of levels.

## Output Format
- Return a single integer representing the minimum hours required for the last staff member to arrive. If it is impossible, return -1.

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
