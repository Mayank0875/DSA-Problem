## Title
Chain of Command

## Slug
chain-of-command

## Difficulty
Medium

## Description
Orders are passed down? No, reports are passed up to the General.

There are $n$ officers numbered from $1$ to $n$, connected by $n-1$ communication lines. The network forms a tree structure (there is exactly one path between any two officers). Currently, all communication lines are one-way.

The hierarchy demands info flow to the **General (Node 1)**. To ensure success, every other officer must be able to reach General by traveling along the communication lines in the correct direction.

You are given the current orientation of the communication lines. Your task is to determine the **minimum** number of communication lines that need to be clarified so that every officer can reach General.

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
The destination is General (1).
- Line 1->2 points away from 1. Needs clarification.
- Line 2->4 points away from 1. Needs clarification.
- Line 3->2 points towards 2 (and effectively towards 1). OK.
- Line 5->1 points towards 1. OK.
- Line 5->6 points away from 1 (via 5). Needs clarification.
Total clarifications: 3.

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
Lines 2->3 and 4->5 need to be clarified.

## Input Format
- The first line contains an integer $n$ — the number of officers.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way line from officer $u$ to officer $v$.

## Output Format
- Return a single integer representing the minimum number of communication lines that need to be changed.

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
