## Title
Ant Colony Foraging

## Slug
ant-colony-foraging

## Difficulty
Hard

## Description
Ants carry food from a picnic site back to the queen in the nest. The pheromone trails can only support a steady stream of ants.

The network consists of n waypoints, numbered 1 to n.
1. Waypoint 1 is the Picnic Site.
2. Waypoint n is the Queen's Chamber.

There are m one-way trails connecting these waypoints. Each trail has a specific capacity, measured in ants per second, which limits the rate at which ants can flow through it.

Multiple trails can exist between the same two waypoints, and their capacities stack. Your goal is to determine the maximum total food transport that can be achieved from the Picnic Site to the Queen's Chamber using the available network.

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
There are two main paths to transmit ants from node 1 to node 4:
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
- The first line contains two integers n and m: the number of waypoints and the number of trails.
- The next m lines describe the trails. Each line contains three integers u, v, and c, indicating a one-way trail from Waypoint u to Waypoint v with capacity c.

## Output Format
- Return one integer: the maximum food transport from Waypoint 1 to Waypoint n.

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
