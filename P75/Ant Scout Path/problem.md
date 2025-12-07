## Title
Ant Scout Path

## Slug
ant-scout-path

## Difficulty
Medium

## Description
Ants leave pheromone trails. Sometimes they get confused and walk in circles.

A "death spiral" occurs when an ant moves from a landmark, through a sequence of trails, and returns to the starting landmark without traversing the same trail twice in immediate succession. The "length" of such a death spiral is the number of trails it contains.

You want to find the length of the shortest circular path an ant might get stuck in.

Given the layout of the terrain, determine the length of the shortest death spiral.

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
There are several death spirals in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest death spiral has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no death spirals in this network.

## Input Format
- The first line contains two integers n and m: the number of landmarks and the number of trails.
- The landmarks are numbered 1, 2, ..., n.
- The next m lines describe the trails. Each line contains two integers u and v, indicating a connection between landmark u and landmark v.
- The graph is undirected. There is at most one trail between any two landmarks.

## Output Format
- Return one integer: the length of the shortest death spiral. If there are no death spirals, print `-1`.

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
