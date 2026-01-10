## Title
Ant Colony

## Slug
ant-colony

## Difficulty
Medium

## Description
Ants leave pheromone trails. All trails must lead back to the Queen's Chamber for the food delivery.

There are $n$ chambers numbered from $1$ to $n$, connected by $n-1$ tunnels. The network forms a tree structure (there is exactly one path between any two chambers). Currently, all tunnels are one-way.

The colony needs all paths to lead to the **Queen's Chamber (Node 1)**. To ensure success, every other chamber must be able to reach Queen's Chamber by traveling along the tunnels in the correct direction.

You are given the current orientation of the tunnels. Your task is to determine the **minimum** number of tunnels that need to be marked backwards so that every chamber can reach Queen's Chamber.

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
The destination is Queen's Chamber (1).
- Tunnel 1->2 points away from 1. Needs change.
- Tunnel 2->4 points away from 1. Needs change.
- Tunnel 3->2 points towards 2 (and effectively towards 1). OK.
- Tunnel 5->1 points towards 1. OK.
- Tunnel 5->6 points away from 1 (via 5). Needs change.
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
Tunnels 2->3 and 4->5 need to be changed.

## Input Format
- The first line contains an integer $n$ — the number of chambers.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way tunnel from chamber $u$ to chamber $v$.

## Output Format
- Return a single integer representing the minimum number of tunnels that need to be changed.

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
