## Title
Search Party

## Slug
search-party

## Difficulty
Medium

## Description
Volunteers search a forest. All teams must report back to Base Camp.

There are $n$ landmarks numbered from $1$ to $n$, connected by $n-1$ trails. The network forms a tree structure (there is exactly one path between any two landmarks). Currently, all trails are one-way.

Coordination requires everyone to move to the **Base Camp (Node 1)**. To ensure success, every other landmark must be able to reach Base Camp by traveling along the trails in the correct direction.

You are given the current orientation of the trails. Your task is to determine the **minimum** number of trails that need to be remarked so that every landmark can reach Base Camp.

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
The destination is Base Camp (1).
- Trail 1->2 points away from 1. Needs remarking.
- Trail 2->4 points away from 1. Needs remarking.
- Trail 3->2 points towards 2 (and effectively towards 1). OK.
- Trail 5->1 points towards 1. OK.
- Trail 5->6 points away from 1 (via 5). Needs remarking.
Total remarkings: 3.

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
Trails 2->3 and 4->5 need to be remarked.

## Input Format
- The first line contains an integer $n$ — the number of landmarks.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way trail from landmark $u$ to landmark $v$.

## Output Format
- Return a single integer representing the minimum number of trails that need to be changed.

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
