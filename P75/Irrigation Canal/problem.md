## Title
Irrigation Canal

## Slug
irrigation-canal

## Difficulty
Medium

## Description
Water flows to fields. Recirculation canals save water by looping back to the pump.

A "water cycle" occurs when water moves from a gate, through a sequence of canals, and returns to the starting gate without traversing the same canal twice in immediate succession. The "length" of such a water cycle is the number of canals it contains.

Find the length of the shortest irrigation loop.

Given the layout of the farm, determine the length of the shortest water cycle.

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
There are several water cycles in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest water cycle has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no water cycles in this network.

## Input Format
- The first line contains two integers n and m: the number of gates and the number of canals.
- The gates are numbered 1, 2, ..., n.
- The next m lines describe the canals. Each line contains two integers u and v, indicating a connection between gate u and gate v.
- The graph is undirected. There is at most one canal between any two gates.

## Output Format
- Return one integer: the length of the shortest water cycle. If there are no water cycles, print `-1`.

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
