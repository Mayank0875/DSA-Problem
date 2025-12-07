## Title
Hiking Trail Loop

## Slug
hiking-trail-loop

## Difficulty
Medium

## Description
Park rangers map trails. Hikers prefer loop trails that bring them back to their car without backtracking.

A "loop trail" occurs when a hiker moves from a landmark, through a sequence of trails, and returns to the starting landmark without traversing the same trail twice in immediate succession. The "length" of such a loop trail is the number of trails it contains.

Find the distance (in segments) of the shortest loop trail.

Given the layout of the national park, determine the length of the shortest loop trail.

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
There are several loop trails in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest loop trail has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no loop trails in this network.

## Input Format
- The first line contains two integers n and m: the number of landmarks and the number of trails.
- The landmarks are numbered 1, 2, ..., n.
- The next m lines describe the trails. Each line contains two integers u and v, indicating a connection between landmark u and landmark v.
- The graph is undirected. There is at most one trail between any two landmarks.

## Output Format
- Return one integer: the length of the shortest loop trail. If there are no loop trails, print `-1`.

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
