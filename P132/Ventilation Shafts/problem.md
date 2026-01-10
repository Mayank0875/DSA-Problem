## Title
Ventilation Shafts

## Slug
ventilation-shafts

## Difficulty
Medium

## Description
A building clears smoke. All fans must blow smoke to the Roof Vent.

There are $n$ rooms numbered from $1$ to $n$, connected by $n-1$ shafts. The network forms a tree structure (there is exactly one path between any two rooms). Currently, all shafts are one-way.

Fans push air to the **Roof Vent (Node 1)**. To ensure success, every other room must be able to reach Roof Vent by traveling along the shafts in the correct direction.

You are given the current orientation of the shafts. Your task is to determine the **minimum** number of shafts that need to be reversed so that every room can reach Roof Vent.

## Examples

### 1

#### Input
6
1 2
2 4
3 2
5 1
5 6

#### Output
3

#### Explanation
The destination is Roof Vent (1).
- Shaft 1->2 points away from 1. Needs reversal.
- Shaft 2->4 points away from 1. Needs reversal.
- Shaft 3->2 points towards 2 (and effectively towards 1). OK.
- Shaft 5->1 points towards 1. OK.
- Shaft 5->6 points away from 1 (via 5). Needs reversal.
Total reversals: 3.

### 2

#### Input
5
2 1
2 3
4 3
4 5

#### Output
2

#### Explanation
Shafts 2->3 and 4->5 need to be reversed.

## Input Format
- The first line contains an integer $n$ — the number of rooms.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way shaft from room $u$ to room $v$.

## Output Format
- Return a single integer representing the minimum number of shafts that need to be changed.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ u, v ≤ n
- The graph is guaranteed to be a tree.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
tree, depth-first-search, breadth-first-search, graph

## Company
google, amazon
