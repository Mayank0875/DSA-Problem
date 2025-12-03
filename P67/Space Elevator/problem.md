## Title
Space Elevator

## Slug
space-elevator

## Difficulty
Medium

## Description
A cargo pod starts at the Base Station (1). It moves up through various docking rings to the Apex Station (n).

There are n stations numbered from 1 to n.
    1. Station 1 is the starting point.
    2. Station n is the destination.

Between some stations, there are one-way cables that allow movement from u to v. The system contains no loops (directed acyclic graph), meaning you can only move forward towards the goal.

Your task is to find the total number of distinct ways/paths to travel from Station 1 to Station n. Since the answer can be very large, return the count modulo 1000000007.

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
- The first line contains two integers n and m: the number of stations and the number of cables.
- The next m lines each contain two integers u and v, representing a one-way cable from u to v.

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
