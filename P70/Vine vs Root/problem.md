## Title
Vine vs Root

## Slug
vine-vs-root

## Difficulty
Medium

## Description
A parasitic Vine grows along Branches. A Root fungus grows through Soil. Roots connect trees that aren't touching via Branches.

The forest has n trees numbered from 1 to n.
The Canopy Layer connects specific pairs of trees with direct branches.
The Ground Layer is constructed based on a unique rule:
A direct soil path exists between two trees if and only if there is no branch connecting them.

Moving between any two connected trees takes exactly 1 hour on either network.
Two growths, The Vine and The Fungus, depart from tree 1 at the same time, heading for tree n.

1. The Vine travels only using Canopy Layer.
2. The Fungus travels only using Ground Layer.

To ensure safety, they must never arrive at the same tree at the same time (except for the final tree n).
Your task is to compute the minimum number of hours required for **both** growths to reach tree n — specifically, the time when the slower growth arrives.
If either growth cannot reach tree n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second growth cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of trees and the number of branches.
- The next m lines each contain two integers u and v, representing a branch between trees u and v.
- The graph is bidirectional. There is at most one branch between any pair of trees.

## Output Format
- Return a single integer representing the minimum hours required for the last growth to arrive. If it is impossible, return -1.

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
