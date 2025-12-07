## Title
Ecological Food Web

## Slug
ecological-food-web

## Difficulty
Medium

## Description
Biologists are mapping energy flow. While rare, sometimes energy flows in a cycle (e.g., detritivores feeding plants).

A "cycle" occurs when energy moves from a species, through a sequence of interactions, and returns to the starting species without traversing the same interaction twice in immediate succession. The "length" of such a cycle is the number of interactions it contains.

You want to identify the shortest energy loop in the ecosystem.

Given the layout of the food web, determine the length of the shortest cycle.

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
There are several cycles in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest cycle has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no cycles in this network.

## Input Format
- The first line contains two integers n and m: the number of species and the number of interactions.
- The species are numbered 1, 2, ..., n.
- The next m lines describe the interactions. Each line contains two integers u and v, indicating a connection between species u and species v.
- The graph is undirected. There is at most one interaction between any two species.

## Output Format
- Return one integer: the length of the shortest cycle. If there are no cycles, print `-1`.

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
