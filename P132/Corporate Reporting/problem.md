## Title
Corporate Reporting

## Slug
corporate-reporting

## Difficulty
Medium

## Description
A bureaucracy manages reports. All memos must be forwarded up the chain to the CEO.

There are $n$ managers numbered from $1$ to $n$, connected by $n-1$ reporting lines. The network forms a tree structure (there is exactly one path between any two managers). Currently, all reporting lines are one-way.

Company policy mandates info flow to the **CEO (Node 1)**. To ensure success, every other manager must be able to reach CEO by traveling along the reporting lines in the correct direction.

You are given the current orientation of the reporting lines. Your task is to determine the **minimum** number of reporting lines that need to be restructured so that every manager can reach CEO.

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
The destination is CEO (1).
- Line 1->2 points away from 1. Needs restructure.
- Line 2->4 points away from 1. Needs restructure.
- Line 3->2 points towards 2 (and effectively towards 1). OK.
- Line 5->1 points towards 1. OK.
- Line 5->6 points away from 1 (via 5). Needs restructure.
Total restructures: 3.

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
Lines 2->3 and 4->5 need to be restructured.

## Input Format
- The first line contains an integer $n$ — the number of managers.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way reporting line from manager $u$ to manager $v$.

## Output Format
- Return a single integer representing the minimum number of reporting lines that need to be changed.

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
