## Title
Cloud Microservices

## Slug
cloud-microservices

## Difficulty
Medium

## Description
Services call APIs of others. A Service Mesh is a group of services that depend on each other cyclically.

Two services a and b belong to the same Mesh if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of calls.
In other words, two services are in the same Mesh if they are mutually reachable.

Your task is to: Determine how many Meshes exist in total.

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
The services form two distinct groups where round-trip traversal is possible within each group.
Services {1, 2, 3} form one Mesh.
Path: 1 -> 2 -> 3 -> 1.
Services {4, 5} form another Mesh.
Path: 4 -> 5 -> 4.
Total Meshes: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 services and 1 one-way call.
Call: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Meshes.

## Input Format
- The first line contains two integers n and m: the number of services and calls.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way call from service a to service b.

## Output Format
- Return one integer: the total number of Meshes.

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
