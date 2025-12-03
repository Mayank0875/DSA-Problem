## Title
Domino Effect

## Slug
domino-effect

## Difficulty
Medium

## Description
Domino 1 is pushed over. It hits other dominoes in a chain reaction until the final Domino n falls. Calculate the ways the force can travel.

There are n dominoes numbered from 1 to n.
    1. Domino 1 is the starting point.
    2. Domino n is the destination.

Between some dominoes, there are one-way interactions that allow movement from u to v. The system contains no loops (directed acyclic graph), meaning you can only move forward towards the goal.

Your task is to find the total number of distinct ways/paths to travel from Domino 1 to Domino n. Since the answer can be very large, return the count modulo 1000000007.

## Examples

### 1

#### Input
4 5
1 2
2 4
1 3
3 4
1 4

#### Output
3

#### Explanation
There are 3 distinct paths:
1 -> 2 -> 4
1 -> 3 -> 4
1 -> 4

### 2

#### Input
4 5
1 2
3 4
2 3
1 3
2 4

#### Output
3

#### Explanation
There are 3 distinct paths:
1 -> 2 -> 3 -> 4
1 -> 2 -> 4
1 -> 3 -> 4

## Input Format
- The first line contains two integers n and m: the number of dominoes and the number of interactions.
- The next m lines each contain two integers u and v, representing a one-way interaction from u to v.

## Output Format
- Return a single integer: the number of ways to travel from 1 to n, modulo (1e9 + 7).

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
