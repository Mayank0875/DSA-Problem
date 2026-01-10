## Title
Information Leak

## Slug
information-leak

## Difficulty
Medium

## Description
Spies trace a leak. All clues lead back to the Source.

There are $n$ suspects numbered from $1$ to $n$, connected by $n-1$ leads. The network forms a tree structure (there is exactly one path between any two suspects). Currently, all leads are one-way.

The investigation tracks back to the **Source (Node 1)**. To ensure success, every other suspect must be able to reach Source by traveling along the leads in the correct direction.

You are given the current orientation of the leads. Your task is to determine the **minimum** number of leads that need to be traced so that every suspect can reach Source.

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
The destination is Source (1).
- Lead 1->2 points away from 1. Needs trace.
- Lead 2->4 points away from 1. Needs trace.
- Lead 3->2 points towards 2 (and effectively towards 1). OK.
- Lead 5->1 points towards 1. OK.
- Lead 5->6 points away from 1 (via 5). Needs trace.
Total traces: 3.

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
Leads 2->3 and 4->5 need to be traced.

## Input Format
- The first line contains an integer $n$ — the number of suspects.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way lead from suspect $u$ to suspect $v$.

## Output Format
- Return a single integer representing the minimum number of leads that need to be changed.

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
