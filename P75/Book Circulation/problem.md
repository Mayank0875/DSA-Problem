## Title
Book Circulation

## Slug
book-circulation

## Difficulty
Medium

## Description
Library books are passed between branches. If a book returns to a branch it visited, it completed a circuit.

A "circulation circuit" occurs when a book moves from a branch, through a sequence of vans, and returns to the starting branch without traversing the same delivery van twice in immediate succession. The "length" of such a circulation circuit is the number of vans it contains.

Find the length of the shortest circulation circuit.

Given the layout of the library network, determine the length of the shortest circulation circuit.

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
There are several circulation circuits in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest circulation circuit has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no circulation circuits in this network.

## Input Format
- The first line contains two integers n and m: the number of branches and the number of vans.
- The branches are numbered 1, 2, ..., n.
- The next m lines describe the vans. Each line contains two integers u and v, indicating a connection between branch u and branch v.
- The graph is undirected. There is at most one delivery van between any two branches.

## Output Format
- Return one integer: the length of the shortest circulation circuit. If there are no circulation circuits, print `-1`.

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
