## Title
Fire and Ice Routes

## Slug
fire-and-ice-routes

## Difficulty
Medium

## Description
An Elemental Race takes place. The Fire Elemental uses Lava Flows, while the Ice Elemental uses Frozen Paths. Frozen Paths exist where Lava Flows do not.

The elemental plane has n sanctuaries numbered from 1 to n.
The Lava Network connects specific pairs of sanctuaries with direct lava flows.
The Ice Network is constructed based on a unique rule:
A direct frozen path exists between two sanctuaries if and only if there is no lava flow connecting them.

Moving between any two connected sanctuaries takes exactly 1 hour on either network.
Two elementals, The Fire Elemental and The Ice Elemental, depart from sanctuary 1 at the same time, heading for sanctuary n.

1. The Fire Elemental travels only using Lava Network.
2. The Ice Elemental travels only using Ice Network.

To ensure safety, they must never arrive at the same sanctuary at the same time (except for the final sanctuary n).
Your task is to compute the minimum number of hours required for **both** elementals to reach sanctuary n — specifically, the time when the slower elemental arrives.
If either elemental cannot reach sanctuary n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second elemental cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of sanctuaries and the number of lava flows.
- The next m lines each contain two integers u and v, representing a lava flow between sanctuaries u and v.
- The graph is bidirectional. There is at most one lava flow between any pair of sanctuaries.

## Output Format
- Return a single integer representing the minimum hours required for the last elemental to arrive. If it is impossible, return -1.

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
