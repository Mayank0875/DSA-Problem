## Title
Traffic Roundabout

## Slug
traffic-roundabout

## Difficulty
Medium

## Description
City planners are analyzing the road network for potential congestion circles. A traffic loop allows cars to drive endlessly without turning around.

A "loop" occurs when a car moves from a intersection, through a sequence of roads, and returns to the starting intersection without traversing the same road twice in immediate succession. The "length" of such a loop is the number of roads it contains.

Short loops cause rapid congestion. Your task is to identify the shortest circular route in the city.

Given the layout of the road network, determine the length of the shortest loop.

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
- The first line contains two integers n and m: the number of intersections and the number of roads.
- The intersections are numbered 1, 2, ..., n.
- The next m lines describe the roads. Each line contains two integers u and v, indicating a connection between intersection u and intersection v.
- The graph is undirected. There is at most one road between any two intersections.

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
