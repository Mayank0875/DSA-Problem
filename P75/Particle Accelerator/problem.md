## Title
Particle Accelerator

## Slug
particle-accelerator

## Difficulty
Medium

## Description
Particles are accelerated in rings. Magnets bend the beam in a circle.

A "cyclotron ring" occurs when a proton moves from a magnet, through a sequence of pipes, and returns to the starting magnet without traversing the same beam pipe twice in immediate succession. The "length" of such a cyclotron ring is the number of pipes it contains.

Find the circumference (in segments) of the smallest accelerator ring.

Given the layout of the lab, determine the length of the shortest cyclotron ring.

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
There are several cyclotron rings in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest cyclotron ring has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no cyclotron rings in this network.

## Input Format
- The first line contains two integers n and m: the number of magnets and the number of pipes.
- The magnets are numbered 1, 2, ..., n.
- The next m lines describe the pipes. Each line contains two integers u and v, indicating a connection between magnet u and magnet v.
- The graph is undirected. There is at most one beam pipe between any two magnets.

## Output Format
- Return one integer: the length of the shortest cyclotron ring. If there are no cyclotron rings, print `-1`.

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
