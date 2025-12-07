## Title
Theme Park Lines

## Slug
theme-park-lines

## Difficulty
Hard

## Description
Visitors move from the entrance to the main attraction. The pathways and security checks act as bottlenecks.

The network consists of n plazas, numbered 1 to n.
1. Plaza 1 is the Entrance.
2. Plaza n is the Ride.

There are m one-way pathways connecting these plazas. Each pathway has a specific capacity, measured in guests per minute, which limits the rate at which visitors can flow through it.

Multiple pathways can exist between the same two plazas, and their capacities stack. Your goal is to determine the maximum total crowd flow that can be achieved from the Entrance to the Ride using the available network.

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
There are two main paths to transmit visitors from node 1 to node 4:
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
- The first line contains two integers n and m: the number of plazas and the number of pathways.
- The next m lines describe the pathways. Each line contains three integers u, v, and c, indicating a one-way pathway from Plaza u to Plaza v with capacity c.

## Output Format
- Return one integer: the maximum crowd flow from Plaza 1 to Plaza n.

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
