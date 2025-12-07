## Title
Blood Shunt

## Slug
blood-shunt

## Difficulty
Medium

## Description
Doctors analyze blood vessels. A shunt creates a short loop bypassing tissues.

A "circulation loop" occurs when blood moves from a junction, through a sequence of vessels, and returns to the starting junction without traversing the same vessel twice in immediate succession. The "length" of such a circulation loop is the number of vessels it contains.

Short loops can be dangerous. Find the length of the shortest circulatory path.

Given the layout of the vascular system, determine the length of the shortest circulation loop.

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
There are several circulation loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest circulation loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no circulation loops in this network.

## Input Format
- The first line contains two integers n and m: the number of junctions and the number of vessels.
- The junctions are numbered 1, 2, ..., n.
- The next m lines describe the vessels. Each line contains two integers u and v, indicating a connection between junction u and junction v.
- The graph is undirected. There is at most one vessel between any two junctions.

## Output Format
- Return one integer: the length of the shortest circulation loop. If there are no circulation loops, print `-1`.

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
