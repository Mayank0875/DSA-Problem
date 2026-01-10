## Title
Sewer Drainage

## Slug
sewer-drainage

## Difficulty
Medium

## Description
A city engineer maps the sewers. All waste must flow to the Treatment Plant.

There are $n$ junctions numbered from $1$ to $n$, connected by $n-1$ pipes. The network forms a tree structure (there is exactly one path between any two junctions). Currently, all pipes are one-way.

Sanitation requires flow to the **Treatment Plant (Node 1)**. To ensure success, every other junction must be able to reach Treatment Plant by traveling along the pipes in the correct direction.

You are given the current orientation of the pipes. Your task is to determine the **minimum** number of pipes that need to be re-sloped so that every junction can reach Treatment Plant.

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
The destination is Treatment Plant (1).
- Pipe 1->2 points away from 1. Needs re-sloping.
- Pipe 2->4 points away from 1. Needs re-sloping.
- Pipe 3->2 points towards 2 (and effectively towards 1). OK.
- Pipe 5->1 points towards 1. OK.
- Pipe 5->6 points away from 1 (via 5). Needs re-sloping.
Total re-slopings: 3.

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
Pipes 2->3 and 4->5 need to be re-sloped.

## Input Format
- The first line contains an integer $n$ — the number of junctions.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way pipe from junction $u$ to junction $v$.

## Output Format
- Return a single integer representing the minimum number of pipes that need to be changed.

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
