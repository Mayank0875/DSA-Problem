## Title
Satellite Orbit Sync

## Slug
satellite-orbit-sync

## Difficulty
Medium

## Description
Satellites relay signals. A signal loop occurs if a message is relayed back to the sender.

A "relay loop" occurs when a signal moves from a satellite, through a sequence of links, and returns to the starting satellite without traversing the same laser link twice in immediate succession. The "length" of such a relay loop is the number of links it contains.

Loops waste bandwidth. Find the number of hops in the shortest relay loop.

Given the layout of the constellation, determine the length of the shortest relay loop.

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
There are several relay loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest relay loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no relay loops in this network.

## Input Format
- The first line contains two integers n and m: the number of satellites and the number of links.
- The satellites are numbered 1, 2, ..., n.
- The next m lines describe the links. Each line contains two integers u and v, indicating a connection between satellite u and satellite v.
- The graph is undirected. There is at most one laser link between any two satellites.

## Output Format
- Return one integer: the length of the shortest relay loop. If there are no relay loops, print `-1`.

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
