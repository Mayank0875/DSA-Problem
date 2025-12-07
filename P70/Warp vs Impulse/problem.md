## Title
Warp vs Impulse

## Slug
warp-vs-impulse

## Difficulty
Medium

## Description
A Starship uses Warp Drive. A Shuttle uses Impulse. Shuttles travel between stars not connected by Warp Lanes.

The galaxy has n stars numbered from 1 to n.
The Warp Grid connects specific pairs of stars with direct warp lanes.
The Impulse Grid is constructed based on a unique rule:
A direct impulse trajectory exists between two stars if and only if there is no warp lane connecting them.

Moving between any two connected stars takes exactly 1 hour on either network.
Two ships, The Starship and The Shuttle, depart from star 1 at the same time, heading for star n.

1. The Starship travels only using Warp Grid.
2. The Shuttle travels only using Impulse Grid.

To ensure safety, they must never arrive at the same star at the same time (except for the final star n).
Your task is to compute the minimum number of hours required for **both** ships to reach star n — specifically, the time when the slower ship arrives.
If either ship cannot reach star n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second ship cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of stars and the number of warp lanes.
- The next m lines each contain two integers u and v, representing a warp lane between stars u and v.
- The graph is bidirectional. There is at most one warp lane between any pair of stars.

## Output Format
- Return a single integer representing the minimum hours required for the last ship to arrive. If it is impossible, return -1.

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
