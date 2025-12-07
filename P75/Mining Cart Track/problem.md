## Title
Mining Cart Track

## Slug
mining-cart-track

## Difficulty
Medium

## Description
Carts move ore. Tracks form loops to allow continuous hauling.

A "haul loop" occurs when a cart moves from a tunnel junction, through a sequence of rails, and returns to the starting tunnel junction without traversing the same rail twice in immediate succession. The "length" of such a haul loop is the number of rails it contains.

Find the length of the shortest haul loop.

Given the layout of the mine, determine the length of the shortest haul loop.

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
There are several haul loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest haul loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no haul loops in this network.

## Input Format
- The first line contains two integers n and m: the number of junctions and the number of rails.
- The junctions are numbered 1, 2, ..., n.
- The next m lines describe the rails. Each line contains two integers u and v, indicating a connection between tunnel junction u and tunnel junction v.
- The graph is undirected. There is at most one rail between any two junctions.

## Output Format
- Return one integer: the length of the shortest haul loop. If there are no haul loops, print `-1`.

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
