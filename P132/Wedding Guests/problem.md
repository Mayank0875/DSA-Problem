## Title
Wedding Guests

## Slug
wedding-guests

## Difficulty
Medium

## Description
Guests drive from hotels. All cars must arrive at the Reception Hall.

There are $n$ hotels numbered from $1$ to $n$, connected by $n-1$ highways. The network forms a tree structure (there is exactly one path between any two hotels). Currently, all highways are one-way.

The celebration requires travel to the **Reception Hall (Node 1)**. To ensure success, every other hotel must be able to reach Reception Hall by traveling along the highways in the correct direction.

You are given the current orientation of the highways. Your task is to determine the **minimum** number of highways that need to be detoured so that every hotel can reach Reception Hall.

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
The destination is Reception Hall (1).
- Highway 1->2 points away from 1. Needs detour.
- Highway 2->4 points away from 1. Needs detour.
- Highway 3->2 points towards 2 (and effectively towards 1). OK.
- Highway 5->1 points towards 1. OK.
- Highway 5->6 points away from 1 (via 5). Needs detour.
Total detours: 3.

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
Highways 2->3 and 4->5 need to be detoured.

## Input Format
- The first line contains an integer $n$ — the number of hotels.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way highway from hotel $u$ to hotel $v$.

## Output Format
- Return a single integer representing the minimum number of highways that need to be changed.

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
