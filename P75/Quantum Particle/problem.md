## Title
Quantum Particle

## Slug
quantum-particle

## Difficulty
Medium

## Description
Physicists trace particle paths. A particle can enter a closed timelike curve.

A "closed curve" occurs when a boson moves from a state, through a sequence of transitions, and returns to the starting state without traversing the same transition twice in immediate succession. The "length" of such a closed curve is the number of transitions it contains.

Find the smallest quantum loop.

Given the layout of the quantum field, determine the length of the shortest closed curve.

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
There are several closed curves in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest closed curve has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no closed curves in this network.

## Input Format
- The first line contains two integers n and m: the number of states and the number of transitions.
- The states are numbered 1, 2, ..., n.
- The next m lines describe the transitions. Each line contains two integers u and v, indicating a connection between state u and state v.
- The graph is undirected. There is at most one transition between any two states.

## Output Format
- Return one integer: the length of the shortest closed curve. If there are no closed curves, print `-1`.

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
