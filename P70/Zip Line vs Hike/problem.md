## Title
Zip Line vs Hike

## Slug
zip-line-vs-hike

## Difficulty
Medium

## Description
Tourists Zip Line between towers. Hikers walk trails. Trails connect towers not linked by a Zip Line.

The adventure park has n towers numbered from 1 to n.
The Zip Net connects specific pairs of towers with direct lines.
The Trail Net is constructed based on a unique rule:
A direct path exists between two towers if and only if there is no line connecting them.

Moving between any two connected towers takes exactly 1 hour on either network.
Two tourists, The Zipper and The Hiker, depart from tower 1 at the same time, heading for tower n.

1. The Zipper travels only using Zip Net.
2. The Hiker travels only using Trail Net.

To ensure safety, they must never arrive at the same tower at the same time (except for the final tower n).
Your task is to compute the minimum number of hours required for **both** tourists to reach tower n — specifically, the time when the slower tourist arrives.
If either tourist cannot reach tower n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second tourist cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of towers and the number of lines.
- The next m lines each contain two integers u and v, representing a line between towers u and v.
- The graph is bidirectional. There is at most one line between any pair of towers.

## Output Format
- Return a single integer representing the minimum hours required for the last tourist to arrive. If it is impossible, return -1.

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
