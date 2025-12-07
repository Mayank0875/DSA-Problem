## Title
Recursion Depth

## Slug
recursion-depth

## Difficulty
Medium

## Description
A program has functions calling each other. Indirect recursion happens when A calls B, which calls A.

A "recursion loop" occurs when execution moves from a function, through a sequence of calls, and returns to the starting function without traversing the same call twice in immediate succession. The "length" of such a recursion loop is the number of calls it contains.

Short recursion loops can cause stack overflow. Find the shortest recursion chain.

Given the layout of the codebase, determine the length of the shortest recursion loop.

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
There are several recursion loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest recursion loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no recursion loops in this network.

## Input Format
- The first line contains two integers n and m: the number of functions and the number of calls.
- The functions are numbered 1, 2, ..., n.
- The next m lines describe the calls. Each line contains two integers u and v, indicating a connection between function u and function v.
- The graph is undirected. There is at most one call between any two functions.

## Output Format
- Return one integer: the length of the shortest recursion loop. If there are no recursion loops, print `-1`.

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
