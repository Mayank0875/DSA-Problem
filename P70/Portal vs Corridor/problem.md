## Title
Portal vs Corridor

## Slug
portal-vs-corridor

## Difficulty
Medium

## Description
Test Subjects use Portals. Researchers use Corridors. Corridors connect test chambers not linked by a Portal.

The lab has n chambers numbered from 1 to n.
The Portal Net connects specific pairs of chambers with direct portals.
The Hallway Net is constructed based on a unique rule:
A direct hallway exists between two chambers if and only if there is no portal connecting them.

Moving between any two connected chambers takes exactly 1 hour on either network.
Two runners, The Subject and The Researcher, depart from chamber 1 at the same time, heading for chamber n.

1. The Subject travels only using Portal Net.
2. The Researcher travels only using Hallway Net.

To ensure safety, they must never arrive at the same chamber at the same time (except for the final chamber n).
Your task is to compute the minimum number of hours required for **both** runners to reach chamber n — specifically, the time when the slower runner arrives.
If either runner cannot reach chamber n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second runner cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of chambers and the number of portals.
- The next m lines each contain two integers u and v, representing a portal between chambers u and v.
- The graph is bidirectional. There is at most one portal between any pair of chambers.

## Output Format
- Return a single integer representing the minimum hours required for the last runner to arrive. If it is impossible, return -1.

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
