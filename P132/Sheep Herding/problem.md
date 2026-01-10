## Title
Sheep Herding

## Slug
sheep-herding

## Difficulty
Medium

## Description
A shepherd moves sheep through pastures. All sheep must be driven to the Barn.

There are $n$ pastures numbered from $1$ to $n$, connected by $n-1$ gates. The network forms a tree structure (there is exactly one path between any two pastures). Currently, all gates are one-way.

The dogs must guide the flock to the **Barn (Node 1)**. To ensure success, every other pasture must be able to reach Barn by traveling along the gates in the correct direction.

You are given the current orientation of the gates. Your task is to determine the **minimum** number of gates that need to be opened differently so that every pasture can reach Barn.

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
The destination is Barn (1).
- Gate 1->2 points away from 1. Needs change.
- Gate 2->4 points away from 1. Needs change.
- Gate 3->2 points towards 2 (and effectively towards 1). OK.
- Gate 5->1 points towards 1. OK.
- Gate 5->6 points away from 1 (via 5). Needs change.
Total changes: 3.

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
Gates 2->3 and 4->5 need to be changed.

## Input Format
- The first line contains an integer $n$ — the number of pastures.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way gate from pasture $u$ to pasture $v$.

## Output Format
- Return a single integer representing the minimum number of gates that need to be changed.

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
