## Title
Ship vs Submarine

## Slug
ship-vs-submarine

## Difficulty
Medium

## Description
A Surface Ship uses Open Water lanes. A Submarine uses Deep Trenches. Trenches connect coordinates that Open Water lanes don't cover.

The ocean has n buoys numbered from 1 to n.
The Surface Route connects specific pairs of buoys with direct lanes.
The Deep Route is constructed based on a unique rule:
A direct trench exists between two buoys if and only if there is no lane connecting them.

Moving between any two connected buoys takes exactly 1 hour on either network.
Two vessels, The Ship and The Sub, depart from buoy 1 at the same time, heading for buoy n.

1. The Ship travels only using Surface Route.
2. The Sub travels only using Deep Route.

To ensure safety, they must never arrive at the same buoy at the same time (except for the final buoy n).
Your task is to compute the minimum number of hours required for **both** vessels to reach buoy n — specifically, the time when the slower vessel arrives.
If either vessel cannot reach buoy n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second vessel cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of buoys and the number of lanes.
- The next m lines each contain two integers u and v, representing a lane between buoys u and v.
- The graph is bidirectional. There is at most one lane between any pair of buoys.

## Output Format
- Return a single integer representing the minimum hours required for the last vessel to arrive. If it is impossible, return -1.

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
