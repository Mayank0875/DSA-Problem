## Title
Owl vs Mole

## Slug
owl-vs-mole

## Difficulty
Medium

## Description
An Owl flies between Treetops. A Mole digs between Burrows. Burrows connect locations not linked by Treetops.

The woodland has n landmarks numbered from 1 to n.
The Sky Route connects specific pairs of landmarks with direct flight lines.
The Underground Route is constructed based on a unique rule:
A direct tunnel exists between two landmarks if and only if there is no flight line connecting them.

Moving between any two connected landmarks takes exactly 1 hour on either network.
Two creatures, The Owl and The Mole, depart from landmark 1 at the same time, heading for landmark n.

1. The Owl travels only using Sky Route.
2. The Mole travels only using Underground Route.

To ensure safety, they must never arrive at the same landmark at the same time (except for the final landmark n).
Your task is to compute the minimum number of hours required for **both** creatures to reach landmark n — specifically, the time when the slower creature arrives.
If either creature cannot reach landmark n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second creature cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of landmarks and the number of flight lines.
- The next m lines each contain two integers u and v, representing a flight line between landmarks u and v.
- The graph is bidirectional. There is at most one flight line between any pair of landmarks.

## Output Format
- Return a single integer representing the minimum hours required for the last creature to arrive. If it is impossible, return -1.

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
