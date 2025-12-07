## Title
Electrical Short

## Slug
electrical-short

## Difficulty
Medium

## Description
An electrician looks for ground loops in a wiring diagram. These loops cause interference.

A "ground loop" occurs when current moves from a terminal, through a sequence of wires, and returns to the starting terminal without traversing the same wire twice in immediate succession. The "length" of such a ground loop is the number of wires it contains.

Small loops pick up the most noise. Find the girth of the wiring graph.

Given the layout of the circuit, determine the length of the shortest ground loop.

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
There are several ground loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest ground loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no ground loops in this network.

## Input Format
- The first line contains two integers n and m: the number of terminals and the number of wires.
- The terminals are numbered 1, 2, ..., n.
- The next m lines describe the wires. Each line contains two integers u and v, indicating a connection between terminal u and terminal v.
- The graph is undirected. There is at most one wire between any two terminals.

## Output Format
- Return one integer: the length of the shortest ground loop. If there are no ground loops, print `-1`.

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
