## Title
Subway Transfer

## Slug
subway-transfer

## Difficulty
Medium

## Description
A city subway has many lines. A circular line allows passengers to ride indefinitely.

A "circular line" occurs when a train moves from a station, through a sequence of tunnels, and returns to the starting station without traversing the same tunnel twice in immediate succession. The "length" of such a circular line is the number of tunnels it contains.

Find the number of stations in the smallest circular line.

Given the layout of the metro, determine the length of the shortest circular line.

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
There are several circular lines in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest circular line has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no circular lines in this network.

## Input Format
- The first line contains two integers n and m: the number of stations and the number of tunnels.
- The stations are numbered 1, 2, ..., n.
- The next m lines describe the tunnels. Each line contains two integers u and v, indicating a connection between station u and station v.
- The graph is undirected. There is at most one tunnel between any two stations.

## Output Format
- Return one integer: the length of the shortest circular line. If there are no circular lines, print `-1`.

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
