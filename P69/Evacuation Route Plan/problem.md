## Title
Evacuation Route Plan

## Slug
evacuation-route-plan

## Difficulty
Hard

## Description
A stadium must be evacuated to the safe zone. The roads connecting intersections have limits on how many people can pass per minute.

The network consists of n intersections, numbered 1 to n.
1. Intersection 1 is the Stadium.
2. Intersection n is the Safe Zone.

There are m one-way roads connecting these intersections. Each road has a specific capacity, measured in people per minute, which limits the rate at which people can flow through it.

Multiple roads can exist between the same two intersections, and their capacities stack. Your goal is to determine the maximum total evacuation rate that can be achieved from the Stadium to the Safe Zone using the available network.

## Examples

### 1

#### Input
4 5
1 2 3
2 4 2
1 3 4
3 4 5
4 1 3

#### Output
6

#### Explanation
There are two main paths to transmit people from node 1 to node 4:
1 -> 2 -> 4 (capacity limited by link 2 -> 4 with capacity 2).
1 -> 3 -> 4 (capacity limited by link 1 -> 3 with capacity 4).
Total max flow is 2 + 4 = 6. The link 4 -> 1 is ignored because it flows backward from the destination.

### 2

#### Input
3 2
1 2 5
2 3 5

#### Output
5

#### Explanation
A single path 1 -> 2 -> 3 exists with a bottleneck capacity of 5.

## Input Format
- The first line contains two integers n and m: the number of intersections and the number of roads.
- The next m lines describe the roads. Each line contains three integers u, v, and c, indicating a one-way road from Intersection u to Intersection v with capacity c.

## Output Format
- Return one integer: the maximum evacuation rate from Intersection 1 to Intersection n.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ u, v ≤ n
- 1 ≤ c ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
