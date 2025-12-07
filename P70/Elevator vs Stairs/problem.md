## Title
Elevator vs Stairs

## Slug
elevator-vs-stairs

## Difficulty
Medium

## Description
One person takes the Elevator, the other takes the Stairs. Stairs connect floors that the Elevator doesn't service directly.

The skyscraper has n floors numbered from 1 to n.
The Lift Shaft connects specific pairs of floors with direct lift rides.
The Stairwell is constructed based on a unique rule:
A direct stair flight exists between two floors if and only if there is no lift ride connecting them.

Moving between any two connected floors takes exactly 1 hour on either network.
Two people, The Rider and The Walker, depart from floor 1 at the same time, heading for floor n.

1. The Rider travels only using Lift Shaft.
2. The Walker travels only using Stairwell.

To ensure safety, they must never arrive at the same floor at the same time (except for the final floor n).
Your task is to compute the minimum number of hours required for **both** people to reach floor n — specifically, the time when the slower person arrives.
If either person cannot reach floor n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second person cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of floors and the number of lift rides.
- The next m lines each contain two integers u and v, representing a lift ride between floors u and v.
- The graph is bidirectional. There is at most one lift ride between any pair of floors.

## Output Format
- Return a single integer representing the minimum hours required for the last person to arrive. If it is impossible, return -1.

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
