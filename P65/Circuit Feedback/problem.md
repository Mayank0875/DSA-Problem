## Title
Circuit Feedback

## Slug
circuit-feedback

## Difficulty
Medium

## Description
Components connect via wires. A Feedback Loop is a group of components where signal circulates.

Two components a and b belong to the same Feedback Loop if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of wires.
In other words, two components are in the same Feedback Loop if they are mutually reachable.

Your task is to: Determine how many Feedback Loops exist in total.

## Examples

### 1

#### Input
5 6
1 2
2 3
3 1
3 4
4 5
5 4

#### Output
2

#### Explanation
The components form two distinct groups where round-trip traversal is possible within each group.
Components {1, 2, 3} form one Feedback Loop.
Path: 1 -> 2 -> 3 -> 1.
Components {4, 5} form another Feedback Loop.
Path: 4 -> 5 -> 4.
Total Feedback Loops: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 components and 1 one-way wire.
Wire: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Feedback Loops.

## Input Format
- The first line contains two integers n and m: the number of components and wires.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way wire from component a to component b.

## Output Format
- Return one integer: the total number of Feedback Loops.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search
