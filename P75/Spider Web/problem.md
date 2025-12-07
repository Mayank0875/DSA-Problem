## Title
Spider Web

## Slug
spider-web

## Difficulty
Medium

## Description
A spider builds a web. Structural threads form rings to support the sticky spiral.

A "structural ring" occurs when the spider moves from a intersection, through a sequence of threads, and returns to the starting intersection without traversing the same silk thread twice in immediate succession. The "length" of such a structural ring is the number of threads it contains.

Small rings are stronger. Find the size of the smallest ring in the web.

Given the layout of the web, determine the length of the shortest structural ring.

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
There are several structural rings in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest structural ring has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no structural rings in this network.

## Input Format
- The first line contains two integers n and m: the number of intersections and the number of threads.
- The intersections are numbered 1, 2, ..., n.
- The next m lines describe the threads. Each line contains two integers u and v, indicating a connection between intersection u and intersection v.
- The graph is undirected. There is at most one silk thread between any two intersections.

## Output Format
- Return one integer: the length of the shortest structural ring. If there are no structural rings, print `-1`.

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
