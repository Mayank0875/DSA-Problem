## Title
Mining Cart Tracks

## Slug
mining-cart-tracks

## Difficulty
Medium

## Description
An underground mine has a rail system. All ore carts must roll towards the Surface Elevator.

There are $n$ excavation sites numbered from $1$ to $n$, connected by $n-1$ rails. The network forms a tree structure (there is exactly one path between any two excavation sites). Currently, all rails are one-way.

Gravity or engines must push carts to the **Surface Elevator (Node 1)**. To ensure success, every other site must be able to reach Surface Elevator by traveling along the rails in the correct direction.

You are given the current orientation of the rails. Your task is to determine the **minimum** number of rails that need to be switched so that every site can reach Surface Elevator.

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
The destination is Surface Elevator (1).
- Rail 1->2 points away from 1. Needs switch.
- Rail 2->4 points away from 1. Needs switch.
- Rail 3->2 points towards 2 (and effectively towards 1). OK.
- Rail 5->1 points towards 1. OK.
- Rail 5->6 points away from 1 (via 5). Needs switch.
Total switchs: 3.

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
Rails 2->3 and 4->5 need to be switched.

## Input Format
- The first line contains an integer $n$ — the number of excavation sites.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way rail from site $u$ to site $v$.

## Output Format
- Return a single integer representing the minimum number of rails that need to be changed.

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
