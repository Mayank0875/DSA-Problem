## Title
Lazy River

## Slug
lazy-river

## Difficulty
Medium

## Description
A water park designs a tubing course. The river must flow back to the start.

A "river loop" occurs when a floater moves from a pool, through a sequence of channels, and returns to the starting pool without traversing the same channel twice in immediate succession. The "length" of such a river loop is the number of channels it contains.

Find the length of the shortest lazy river route.

Given the layout of the water park, determine the length of the shortest river loop.

## Examples

### 1

#### Input
5 6
1 2
1 3
2 4
2 5
3 4
4 5

#### Output
3

#### Explanation
There are several river loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest river loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no river loops in this network.

## Input Format
- The first line contains two integers n and m: the number of pools and the number of channels.
- The pools are numbered 1, 2, ..., n.
- The next m lines describe the channels. Each line contains two integers u and v, indicating a connection between pool u and pool v.
- The graph is undirected. There is at most one channel between any two pools.

## Output Format
- Return one integer: the length of the shortest river loop. If there are no river loops, print `-1`.

## Constraints
- 1 ≤ n ≤ 2500
- 1 ≤ m ≤ 5000
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
