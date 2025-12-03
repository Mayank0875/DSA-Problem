## Title
Pipeline System

## Slug
pipeline-system

## Difficulty
Hard

## Description
n valves control a factory. Pipes connect some valves into systems. Safety protocols require systems of 'Safe Capacity' (digits 4 and 7).

A plumber can install new pipes. Merging k systems requires k - 1 pipes.

Your task is to determine the minimum number of extra pipes the plumber needs to build to create at least one system whose size is a Safe Capacity. If this goal cannot be achieved, return -1.

## Examples

### 1

#### Input
4 3
1 2
2 3
1 3

#### Output
1

#### Explanation
The optimal way is to connect valve 4 with valve 3. We can also connect 4 with 1 or 2. This creates a system of size 4 (a Safe Capacity).

### 2

#### Input
5 4
1 2
3 4
4 5
3 5

#### Output
-1

#### Explanation
There is no way to connect the valves to form a system with a size equal to a Safe Capacity.

## Input Format
- The first line contains two integers n and m: the number of valves and the number of existing pipes.
- The next m lines each contain two integers u and v, representing a pipe between valve u and valve v. Note that u may be equal to v, and there may be multiple pipes connecting the same pair of valves.

## Output Format
- Return a single integer: the minimum number of pipes to build. If no solution exists, print -1.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming

## Companies
infosys
