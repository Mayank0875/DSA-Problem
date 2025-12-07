## Title
Telescope Array

## Slug
telescope-array

## Difficulty
Medium

## Description
Radio telescopes are linked to synthesize a larger aperture. Data must sync in a loop.

A "sync loop" occurs when data stream moves from a dish, through a sequence of links, and returns to the starting dish without traversing the same fiber link twice in immediate succession. The "length" of such a sync loop is the number of links it contains.

Short loops reduce latency. Find the size of the smallest sync loop.

Given the layout of the array, determine the length of the shortest sync loop.

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
There are several sync loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest sync loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no sync loops in this network.

## Input Format
- The first line contains two integers n and m: the number of dishes and the number of links.
- The dishes are numbered 1, 2, ..., n.
- The next m lines describe the links. Each line contains two integers u and v, indicating a connection between dish u and dish v.
- The graph is undirected. There is at most one fiber link between any two dishes.

## Output Format
- Return one integer: the length of the shortest sync loop. If there are no sync loops, print `-1`.

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
