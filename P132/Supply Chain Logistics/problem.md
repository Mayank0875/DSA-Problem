## Title
Supply Chain Logistics

## Slug
supply-chain-logistics

## Difficulty
Medium

## Description
A manufacturing giant has many factories. All raw materials must eventually reach the Final Assembly Plant.

There are $n$ factories numbered from $1$ to $n$, connected by $n-1$ conveyor belts. The network forms a tree structure (there is exactly one path between any two factories). Currently, all conveyor belts are one-way.

Logistics demand all goods move to the **Final Assembly Plant (Node 1)**. To ensure success, every other factory must be able to reach Final Assembly Plant by traveling along the conveyor belts in the correct direction.

You are given the current orientation of the conveyor belts. Your task is to determine the **minimum** number of conveyor belts that need to be reversed so that every factory can reach Final Assembly Plant.

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
The destination is Final Assembly Plant (1).
- Belt 1->2 points away from 1. Needs reversal.
- Belt 2->4 points away from 1. Needs reversal.
- Belt 3->2 points towards 2 (and effectively towards 1). OK.
- Belt 5->1 points towards 1. OK.
- Belt 5->6 points away from 1 (via 5). Needs reversal.
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
Belts 2->3 and 4->5 need to be reversed.

## Input Format
- The first line contains an integer $n$ — the number of factories.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way conveyor belt from factory $u$ to factory $v$.

## Output Format
- Return a single integer representing the minimum number of conveyor belts that need to be changed.

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
