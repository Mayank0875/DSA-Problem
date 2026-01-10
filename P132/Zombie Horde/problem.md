## Title
Zombie Horde

## Slug
zombie-horde

## Difficulty
Medium

## Description
Zombies wander the streets. A loud noise attracts them all to the Town Square.

There are $n$ blocks numbered from $1$ to $n$, connected by $n-1$ streets. The network forms a tree structure (there is exactly one path between any two blocks). Currently, all streets are one-way.

The noise draws them to the **Town Square (Node 1)**. To ensure success, every other block must be able to reach Town Square by traveling along the streets in the correct direction.

You are given the current orientation of the streets. Your task is to determine the **minimum** number of streets that need to be lured so that every block can reach Town Square.

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
The destination is Town Square (1).
- Street 1->2 points away from 1. Needs lure.
- Street 2->4 points away from 1. Needs lure.
- Street 3->2 points towards 2 (and effectively towards 1). OK.
- Street 5->1 points towards 1. OK.
- Street 5->6 points away from 1 (via 5). Needs lure.
Total lures: 3.

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
Streets 2->3 and 4->5 need to be lured.

## Input Format
- The first line contains an integer $n$ — the number of blocks.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way street from block $u$ to block $v$.

## Output Format
- Return a single integer representing the minimum number of streets that need to be changed.

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
