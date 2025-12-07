## Title
Elevator System

## Slug
elevator-system

## Difficulty
Medium

## Description
In a mega-building, elevators and moving walkways form a transit web. A loop allows continuous movement.

A "transit loop" occurs when a passenger moves from a floor lobby, through a sequence of shafts, and returns to the starting floor lobby without traversing the same lift shaft twice in immediate succession. The "length" of such a transit loop is the number of shafts it contains.

Find the smallest transit loop for maintenance testing.

Given the layout of the skyscraper, determine the length of the shortest transit loop.

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
There are several transit loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest transit loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no transit loops in this network.

## Input Format
- The first line contains two integers n and m: the number of lobbies and the number of shafts.
- The lobbies are numbered 1, 2, ..., n.
- The next m lines describe the shafts. Each line contains two integers u and v, indicating a connection between floor lobby u and floor lobby v.
- The graph is undirected. There is at most one lift shaft between any two lobbies.

## Output Format
- Return one integer: the length of the shortest transit loop. If there are no transit loops, print `-1`.

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
