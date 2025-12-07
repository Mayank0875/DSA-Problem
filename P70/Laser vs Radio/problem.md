## Title
Laser vs Radio

## Slug
laser-vs-radio

## Difficulty
Medium

## Description
A Laser Comm system requires line-of-sight. A Radio Comm system works through obstacles. Radio connects points without line-of-sight.

The outpost network has n towers numbered from 1 to n.
The LOS Net connects specific pairs of towers with direct laser beams.
The Non-LOS Net is constructed based on a unique rule:
A direct radio wave exists between two towers if and only if there is no laser beam connecting them.

Moving between any two connected towers takes exactly 1 hour on either network.
Two messages, Laser Message and Radio Message, depart from tower 1 at the same time, heading for tower n.

1. Laser Message travels only using LOS Net.
2. Radio Message travels only using Non-LOS Net.

To ensure safety, they must never arrive at the same tower at the same time (except for the final tower n).
Your task is to compute the minimum number of hours required for **both** messages to reach tower n — specifically, the time when the slower message arrives.
If either message cannot reach tower n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second message cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of towers and the number of laser beams.
- The next m lines each contain two integers u and v, representing a laser beam between towers u and v.
- The graph is bidirectional. There is at most one laser beam between any pair of towers.

## Output Format
- Return a single integer representing the minimum hours required for the last message to arrive. If it is impossible, return -1.

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
