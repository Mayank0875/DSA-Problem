## Title
Fish Migration

## Slug
fish-migration

## Difficulty
Medium

## Description
Salmon swim through a river network. They must reach the Spawning Ground.

There are $n$ pools numbered from $1$ to $n$, connected by $n-1$ rapids. The network forms a tree structure (there is exactly one path between any two pools). Currently, all rapids are one-way.

Instinct drives them to the **Spawning Ground (Node 1)**. To ensure success, every other pool must be able to reach Spawning Ground by traveling along the rapids in the correct direction.

You are given the current orientation of the rapids. Your task is to determine the **minimum** number of rapids that need to be leaped so that every pool can reach Spawning Ground.

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
The destination is Spawning Ground (1).
- Rapid 1->2 points away from 1. Needs leap.
- Rapid 2->4 points away from 1. Needs leap.
- Rapid 3->2 points towards 2 (and effectively towards 1). OK.
- Rapid 5->1 points towards 1. OK.
- Rapid 5->6 points away from 1 (via 5). Needs leap.
Total leaps: 3.

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
Rapids 2->3 and 4->5 need to be leaped.

## Input Format
- The first line contains an integer $n$ — the number of pools.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way rapid from pool $u$ to pool $v$.

## Output Format
- Return a single integer representing the minimum number of rapids that need to be changed.

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
