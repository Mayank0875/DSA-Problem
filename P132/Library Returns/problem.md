## Title
Library Returns

## Slug
library-returns

## Difficulty
Medium

## Description
Automated carts collect books. All carts must roll to the Sorting Desk.

There are $n$ collection points numbered from $1$ to $n$, connected by $n-1$ tracks. The network forms a tree structure (there is exactly one path between any two collection points). Currently, all tracks are one-way.

The system guides books to the **Sorting Desk (Node 1)**. To ensure success, every other collection point must be able to reach Sorting Desk by traveling along the tracks in the correct direction.

You are given the current orientation of the tracks. Your task is to determine the **minimum** number of tracks that need to be switched so that every collection point can reach Sorting Desk.

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
The destination is Sorting Desk (1).
- Track 1->2 points away from 1. Needs switch.
- Track 2->4 points away from 1. Needs switch.
- Track 3->2 points towards 2 (and effectively towards 1). OK.
- Track 5->1 points towards 1. OK.
- Track 5->6 points away from 1 (via 5). Needs switch.
Total switchs: 3.

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
Tracks 2->3 and 4->5 need to be switched.

## Input Format
- The first line contains an integer $n$ — the number of collection points.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way track from collection point $u$ to collection point $v$.

## Output Format
- Return a single integer representing the minimum number of tracks that need to be changed.

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
