## Title
Space Station Corridors

## Slug
space-station-corridors

## Difficulty
Medium

## Description
Astronauts navigate a station. Loops allow for redundant paths in case of decompression.

A "circuit" occurs when an astronaut moves from a module, through a sequence of hallways, and returns to the starting module without traversing the same hallway twice in immediate succession. The "length" of such a circuit is the number of hallways it contains.

Short circuits allow quick movement. Find the length of the shortest loop in the station.

Given the layout of the space station, determine the length of the shortest circuit.

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
There are several circuits in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest circuit has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no circuits in this network.

## Input Format
- The first line contains two integers n and m: the number of modules and the number of hallways.
- The modules are numbered 1, 2, ..., n.
- The next m lines describe the hallways. Each line contains two integers u and v, indicating a connection between module u and module v.
- The graph is undirected. There is at most one hallway between any two modules.

## Output Format
- Return one integer: the length of the shortest circuit. If there are no circuits, print `-1`.

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
