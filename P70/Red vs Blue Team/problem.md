## Title
Red vs Blue Team

## Slug
red-vs-blue-team

## Difficulty
Medium

## Description
In a capture-the-flag game, Red Team uses Red Tunnels and Blue Team uses Blue Bridges. Blue Bridges connect bases that are not connected by Red Tunnels.

The battlefield has n bases numbered from 1 to n.
The Red Network connects specific pairs of bases with direct tunnels.
The Blue Network is constructed based on a unique rule:
A direct bridge exists between two bases if and only if there is no tunnel connecting them.

Moving between any two connected bases takes exactly 1 hour on either network.
Two scouts, The Red Scout and The Blue Scout, depart from base 1 at the same time, heading for base n.

1. The Red Scout travels only using Red Network.
2. The Blue Scout travels only using Blue Network.

To ensure safety, they must never arrive at the same base at the same time (except for the final base n).
Your task is to compute the minimum number of hours required for **both** scouts to reach base n — specifically, the time when the slower scout arrives.
If either scout cannot reach base n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second scout cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of bases and the number of tunnels.
- The next m lines each contain two integers u and v, representing a tunnel between bases u and v.
- The graph is bidirectional. There is at most one tunnel between any pair of bases.

## Output Format
- Return a single integer representing the minimum hours required for the last scout to arrive. If it is impossible, return -1.

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
