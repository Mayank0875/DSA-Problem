## Title
Plumbing Backflow

## Slug
plumbing-backflow

## Difficulty
Medium

## Description
A plumber inspects a pipe network. A loop can cause pressure issues and backflow.

A "loop" occurs when water moves from a joint, through a sequence of pipes, and returns to the starting joint without traversing the same pipe twice in immediate succession. The "length" of such a loop is the number of pipes it contains.

Short loops cause the most pressure variance. Find the length of the smallest pipe loop.

Given the layout of the plumbing system, determine the length of the shortest loop.

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
There are several loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no loops in this network.

## Input Format
- The first line contains two integers n and m: the number of joints and the number of pipes.
- The joints are numbered 1, 2, ..., n.
- The next m lines describe the pipes. Each line contains two integers u and v, indicating a connection between joint u and joint v.
- The graph is undirected. There is at most one pipe between any two joints.

## Output Format
- Return one integer: the length of the shortest loop. If there are no loops, print `-1`.

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
