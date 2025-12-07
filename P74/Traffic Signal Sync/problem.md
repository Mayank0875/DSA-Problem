## Title
Traffic Signal Sync

## Slug
traffic-signal-sync

## Difficulty
Medium

## Description
Intersections in a suburb form a tree. Traffic engineers want to synchronize adjacent signals in pairs to optimize flow. Each signal can be synced with one neighbor.

The structure is a tree with n intersections and n-1 roads.
A synced pair is formed between two intersections connected by a road.
However, each intersection can be part of at most one synced pair.

Your task is to calculate the maximum number of synced pairs that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of synced pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 synced pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form synced pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of intersections.
- The next n-1 lines each contain two integers u and v, representing a road between intersection u and intersection v.

## Output Format
- Return a single integer representing the maximum number of synced pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
