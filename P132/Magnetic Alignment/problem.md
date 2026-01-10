## Title
Magnetic Alignment

## Slug
magnetic-alignment

## Difficulty
Medium

## Description
Iron filings align on paper. They must all point to the North Pole magnet.

There are $n$ filing clusters numbered from $1$ to $n$, connected by $n-1$ field lines. The network forms a tree structure (there is exactly one path between any two filing clusters). Currently, all field lines are one-way.

Magnetism aligns them to the **North Pole (Node 1)**. To ensure success, every other cluster must be able to reach North Pole by traveling along the field lines in the correct direction.

You are given the current orientation of the field lines. Your task is to determine the **minimum** number of field lines that need to be flipped so that every cluster can reach North Pole.

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
The destination is North Pole (1).
- Line 1->2 points away from 1. Needs flip.
- Line 2->4 points away from 1. Needs flip.
- Line 3->2 points towards 2 (and effectively towards 1). OK.
- Line 5->1 points towards 1. OK.
- Line 5->6 points away from 1 (via 5). Needs flip.
Total flips: 3.

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
Lines 2->3 and 4->5 need to be flipped.

## Input Format
- The first line contains an integer $n$ — the number of filing clusters.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way field line from cluster $u$ to cluster $v$.

## Output Format
- Return a single integer representing the minimum number of field lines that need to be changed.

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
