## Title
Express vs Local

## Slug
express-vs-local

## Difficulty
Medium

## Description
An Express Train uses fast tracks. A Local Tram uses street rails. Street rails connect stops that the fast tracks skip (don't connect).

The transit map has n stops numbered from 1 to n.
The Express Line connects specific pairs of stops with direct fast tracks.
The Local Line is constructed based on a unique rule:
A direct street rail exists between two stops if and only if there is no fast track connecting them.

Moving between any two connected stops takes exactly 1 hour on either network.
Two trains, The Express and The Local, depart from stop 1 at the same time, heading for stop n.

1. The Express travels only using Express Line.
2. The Local travels only using Local Line.

To ensure safety, they must never arrive at the same stop at the same time (except for the final stop n).
Your task is to compute the minimum number of hours required for **both** trains to reach stop n — specifically, the time when the slower train arrives.
If either train cannot reach stop n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second train cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of stops and the number of fast tracks.
- The next m lines each contain two integers u and v, representing a fast track between stops u and v.
- The graph is bidirectional. There is at most one fast track between any pair of stops.

## Output Format
- Return a single integer representing the minimum hours required for the last train to arrive. If it is impossible, return -1.

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
