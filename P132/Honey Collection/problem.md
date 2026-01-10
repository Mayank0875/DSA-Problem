## Title
Honey Collection

## Slug
honey-collection

## Difficulty
Medium

## Description
Bees collect nectar. They must fly back to the Hive Entrance.

There are $n$ flower beds numbered from $1$ to $n$, connected by $n-1$ flight corridors. The network forms a tree structure (there is exactly one path between any two flower beds). Currently, all flight corridors are one-way.

The colony works to bring food to the **Hive Entrance (Node 1)**. To ensure success, every other bed must be able to reach Hive Entrance by traveling along the flight corridors in the correct direction.

You are given the current orientation of the flight corridors. Your task is to determine the **minimum** number of flight corridors that need to be guided so that every bed can reach Hive Entrance.

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
The destination is Hive Entrance (1).
- Corridor 1->2 points away from 1. Needs guide.
- Corridor 2->4 points away from 1. Needs guide.
- Corridor 3->2 points towards 2 (and effectively towards 1). OK.
- Corridor 5->1 points towards 1. OK.
- Corridor 5->6 points away from 1 (via 5). Needs guide.
Total guides: 3.

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
Corridors 2->3 and 4->5 need to be guided.

## Input Format
- The first line contains an integer $n$ — the number of flower beds.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way corridor from bed $u$ to bed $v$.

## Output Format
- Return a single integer representing the minimum number of flight corridors that need to be changed.

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
