## Title
Alpha vs Beta Squad

## Slug
alpha-vs-beta-squad

## Difficulty
Medium

## Description
Alpha Squad takes the Main Roads. Beta Squad takes the Back Alleys. Back Alleys connect checkpoints not linked by Main Roads.

The warzone has n checkpoints numbered from 1 to n.
The Main Route connects specific pairs of checkpoints with direct roads.
The Covert Route is constructed based on a unique rule:
A direct alley exists between two checkpoints if and only if there is no road connecting them.

Moving between any two connected checkpoints takes exactly 1 hour on either network.
Two squads, Alpha and Beta, depart from checkpoint 1 at the same time, heading for checkpoint n.

1. Alpha travels only using Main Route.
2. Beta travels only using Covert Route.

To ensure safety, they must never arrive at the same checkpoint at the same time (except for the final checkpoint n).
Your task is to compute the minimum number of hours required for **both** squads to reach checkpoint n — specifically, the time when the slower squad arrives.
If either squad cannot reach checkpoint n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second squad cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of checkpoints and the number of roads.
- The next m lines each contain two integers u and v, representing a road between checkpoints u and v.
- The graph is bidirectional. There is at most one road between any pair of checkpoints.

## Output Format
- Return a single integer representing the minimum hours required for the last squad to arrive. If it is impossible, return -1.

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
