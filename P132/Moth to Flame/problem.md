## Title
Moth to Flame

## Slug
moth-to-flame

## Difficulty
Medium

## Description
Moths fly in a garden. They are all drawn to the Porch Light.

There are $n$ bushes numbered from $1$ to $n$, connected by $n-1$ flight paths. The network forms a tree structure (there is exactly one path between any two bushes). Currently, all flight paths are one-way.

Instinct drives them to the **Porch Light (Node 1)**. To ensure success, every other bush must be able to reach Porch Light by traveling along the flight paths in the correct direction.

You are given the current orientation of the flight paths. Your task is to determine the **minimum** number of flight paths that need to be diverted so that every bush can reach Porch Light.

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
The destination is Porch Light (1).
- Path 1->2 points away from 1. Needs diversion.
- Path 2->4 points away from 1. Needs diversion.
- Path 3->2 points towards 2 (and effectively towards 1). OK.
- Path 5->1 points towards 1. OK.
- Path 5->6 points away from 1 (via 5). Needs diversion.
Total diversions: 3.

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
Paths 2->3 and 4->5 need to be diverted.

## Input Format
- The first line contains an integer $n$ — the number of bushes.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way path from bush $u$ to bush $v$.

## Output Format
- Return a single integer representing the minimum number of flight paths that need to be changed.

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
