## Title
Conveyor Belt Jam

## Slug
conveyor-belt-jam

## Difficulty
Medium

## Description
A factory system recycles items. If items circulate in a short loop, they clog the sorter.

A "recirculation loop" occurs when an item moves from a machine, through a sequence of belts, and returns to the starting machine without traversing the same belt twice in immediate succession. The "length" of such a recirculation loop is the number of belts it contains.

Identify the shortest loop causing immediate jams.

Given the layout of the factory floor, determine the length of the shortest recirculation loop.

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
There are several recirculation loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest recirculation loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no recirculation loops in this network.

## Input Format
- The first line contains two integers n and m: the number of machines and the number of belts.
- The machines are numbered 1, 2, ..., n.
- The next m lines describe the belts. Each line contains two integers u and v, indicating a connection between machine u and machine v.
- The graph is undirected. There is at most one belt between any two machines.

## Output Format
- Return one integer: the length of the shortest recirculation loop. If there are no recirculation loops, print `-1`.

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
