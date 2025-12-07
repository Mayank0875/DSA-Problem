## Title
Treasure Map

## Slug
treasure-map

## Difficulty
Medium

## Description
Pirates hide treasure. Clues lead from one island to another, eventually forming a loop to trap the unworthy.

A "clue chain" occurs when a hunter moves from a island, through a sequence of routes, and returns to the starting island without traversing the same sailing route twice in immediate succession. The "length" of such a clue chain is the number of routes it contains.

Find the length of the shortest clue chain.

Given the layout of the archipelago, determine the length of the shortest clue chain.

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
There are several clue chains in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest clue chain has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no clue chains in this network.

## Input Format
- The first line contains two integers n and m: the number of islands and the number of routes.
- The islands are numbered 1, 2, ..., n.
- The next m lines describe the routes. Each line contains two integers u and v, indicating a connection between island u and island v.
- The graph is undirected. There is at most one sailing route between any two islands.

## Output Format
- Return one integer: the length of the shortest clue chain. If there are no clue chains, print `-1`.

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
