## Title
Ventilation Duct

## Slug
ventilation-duct

## Difficulty
Medium

## Description
HVAC systems need circulation. A return loop recycles air back to the start.

A "air loop" occurs when airflow moves from a vent, through a sequence of ducts, and returns to the starting vent without traversing the same duct twice in immediate succession. The "length" of such a air loop is the number of ducts it contains.

Find the length of the shortest air return loop.

Given the layout of the building, determine the length of the shortest air loop.

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
There are several air loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest air loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no air loops in this network.

## Input Format
- The first line contains two integers n and m: the number of vents and the number of ducts.
- The vents are numbered 1, 2, ..., n.
- The next m lines describe the ducts. Each line contains two integers u and v, indicating a connection between vent u and vent v.
- The graph is undirected. There is at most one duct between any two vents.

## Output Format
- Return one integer: the length of the shortest air loop. If there are no air loops, print `-1`.

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
