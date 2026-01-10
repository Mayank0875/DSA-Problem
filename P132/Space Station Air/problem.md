## Title
Space Station Air

## Slug
space-station-air

## Difficulty
Medium

## Description
A leak occurs! All emergency bulkheads must vent air towards the Life Support module.

There are $n$ modules numbered from $1$ to $n$, connected by $n-1$ vents. The network forms a tree structure (there is exactly one path between any two modules). Currently, all vents are one-way.

Survival depends on air flow to the **Life Support (Node 1)**. To ensure success, every other module must be able to reach Life Support by traveling along the vents in the correct direction.

You are given the current orientation of the vents. Your task is to determine the **minimum** number of vents that need to be forced so that every module can reach Life Support.

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
The destination is Life Support (1).
- Vent 1->2 points away from 1. Needs forcing.
- Vent 2->4 points away from 1. Needs forcing.
- Vent 3->2 points towards 2 (and effectively towards 1). OK.
- Vent 5->1 points towards 1. OK.
- Vent 5->6 points away from 1 (via 5). Needs forcing.
Total forcings: 3.

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
Vents 2->3 and 4->5 need to be forced.

## Input Format
- The first line contains an integer $n$ — the number of modules.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way vent from module $u$ to module $v$.

## Output Format
- Return a single integer representing the minimum number of vents that need to be changed.

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
