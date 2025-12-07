## Title
Ski vs Snowboard

## Slug
ski-vs-snowboard

## Difficulty
Medium

## Description
Skiers use groomed runs. Snowboarders use off-piste. Off-piste connects areas not linked by groomed runs.

The mountain has n lodges numbered from 1 to n.
The Groomed Map connects specific pairs of lodges with direct runs.
The Off-Piste Map is constructed based on a unique rule:
A direct trail exists between two lodges if and only if there is no run connecting them.

Moving between any two connected lodges takes exactly 1 hour on either network.
Two riders, The Skier and The Boarder, depart from lodge 1 at the same time, heading for lodge n.

1. The Skier travels only using Groomed Map.
2. The Boarder travels only using Off-Piste Map.

To ensure safety, they must never arrive at the same lodge at the same time (except for the final lodge n).
Your task is to compute the minimum number of hours required for **both** riders to reach lodge n — specifically, the time when the slower rider arrives.
If either rider cannot reach lodge n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second rider cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of lodges and the number of runs.
- The next m lines each contain two integers u and v, representing a run between lodges u and v.
- The graph is bidirectional. There is at most one run between any pair of lodges.

## Output Format
- Return a single integer representing the minimum hours required for the last rider to arrive. If it is impossible, return -1.

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
