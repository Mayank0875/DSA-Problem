## Title
Teleporter Pads

## Slug
teleporter-pads

## Difficulty
Medium

## Description
Teleporter pads send travelers one way. A Travel Hub is a collection of pads that allow full traversal within the group.

Two pads a and b belong to the same Travel Hub if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of beams.
In other words, two pads are in the same Travel Hub if they are mutually reachable.

Your task is to: Determine how many Travel Hubs exist in total.

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
The pads form two distinct groups where round-trip traversal is possible within each group.
Pads {1, 2, 3} form one Travel Hub.
Path: 1 -> 2 -> 3 -> 1.
Pads {4, 5} form another Travel Hub.
Path: 4 -> 5 -> 4.
Total Travel Hubs: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 pads and 1 one-way beam.
Beam: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Travel Hubs.

## Input Format
- The first line contains two integers n and m: the number of pads and beams.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way beam from pad a to pad b.

## Output Format
- Return one integer: the total number of Travel Hubs.

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
