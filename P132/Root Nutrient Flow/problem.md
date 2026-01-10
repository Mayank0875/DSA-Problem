## Title
Root Nutrient Flow

## Slug
root-nutrient-flow

## Difficulty
Medium

## Description
A tree absorbs water. Nutrients travel from root tips to the Trunk.

There are $n$ root tips numbered from $1$ to $n$, connected by $n-1$ root segments. The network forms a tree structure (there is exactly one path between any two root tips). Currently, all root segments are one-way.

Life depends on flow to the **Trunk (Node 1)**. To ensure success, every other tip must be able to reach Trunk by traveling along the root segments in the correct direction.

You are given the current orientation of the root segments. Your task is to determine the **minimum** number of root segments that need to be osmosis-reversed so that every tip can reach Trunk.

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
The destination is Trunk (1).
- Segment 1->2 points away from 1. Needs reversal.
- Segment 2->4 points away from 1. Needs reversal.
- Segment 3->2 points towards 2 (and effectively towards 1). OK.
- Segment 5->1 points towards 1. OK.
- Segment 5->6 points away from 1 (via 5). Needs reversal.
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
Segments 2->3 and 4->5 need to be reversed.

## Input Format
- The first line contains an integer $n$ — the number of root tips.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way segment from tip $u$ to tip $v$.

## Output Format
- Return a single integer representing the minimum number of root segments that need to be changed.

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
