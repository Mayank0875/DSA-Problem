## Title
Pizza Delivery Return

## Slug
pizza-delivery-return

## Difficulty
Medium

## Description
It's closing time. All delivery drivers must return to the Pizza Shop.

There are $n$ neighborhoods numbered from $1$ to $n$, connected by $n-1$ roads. The network forms a tree structure (there is exactly one path between any two neighborhoods). Currently, all roads are one-way.

The shift ends and drivers drive to the **Pizza Shop (Node 1)**. To ensure success, every other neighborhood must be able to reach Pizza Shop by traveling along the roads in the correct direction.

You are given the current orientation of the roads. Your task is to determine the **minimum** number of roads that need to be u-turned so that every neighborhood can reach Pizza Shop.

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
The destination is Pizza Shop (1).
- Road 1->2 points away from 1. Needs u-turn.
- Road 2->4 points away from 1. Needs u-turn.
- Road 3->2 points towards 2 (and effectively towards 1). OK.
- Road 5->1 points towards 1. OK.
- Road 5->6 points away from 1 (via 5). Needs u-turn.
Total u-turns: 3.

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
Roads 2->3 and 4->5 need to be u-turned.

## Input Format
- The first line contains an integer $n$ — the number of neighborhoods.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way road from neighborhood $u$ to neighborhood $v$.

## Output Format
- Return a single integer representing the minimum number of roads that need to be changed.

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
