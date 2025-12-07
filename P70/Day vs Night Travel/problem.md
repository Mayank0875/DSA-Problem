## Title
Day vs Night Travel

## Slug
day-vs-night-travel

## Difficulty
Medium

## Description
Two adventurers travel across a land. One travels by Day Roads, the other by Night Trails. Night Trails appear only where Day Roads are absent.

The kingdom has n villages numbered from 1 to n.
The Day Network connects specific pairs of villages with direct roads.
The Night Network is constructed based on a unique rule:
A direct trail exists between two villages if and only if there is no road connecting them.

Moving between any two connected villages takes exactly 1 hour on either network.
Two adventurers, The Day Traveler and The Night Walker, depart from village 1 at the same time, heading for village n.

1. The Day Traveler travels only using Day Network.
2. The Night Walker travels only using Night Network.

To ensure safety, they must never arrive at the same village at the same time (except for the final village n).
Your task is to compute the minimum number of hours required for **both** adventurers to reach village n — specifically, the time when the slower adventurer arrives.
If either adventurer cannot reach village n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second adventurer cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of villages and the number of roads.
- The next m lines each contain two integers u and v, representing a road between villages u and v.
- The graph is bidirectional. There is at most one road between any pair of villages.

## Output Format
- Return a single integer representing the minimum hours required for the last adventurer to arrive. If it is impossible, return -1.

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
