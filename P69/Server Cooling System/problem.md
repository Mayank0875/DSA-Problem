## Title
Server Cooling System

## Slug
server-cooling-system

## Difficulty
Hard

## Description
Coolant liquid is pumped from a chiller to the main CPU cluster. The pipes in the rack have flow restrictions.

The network consists of n valves, numbered 1 to n.
1. Valve 1 is the Chiller.
2. Valve n is the CPU Cluster.

There are m one-way pipes connecting these valves. Each pipe has a specific capacity, measured in gallons per minute, which limits the rate at which coolant can flow through it.

Multiple pipes can exist between the same two valves, and their capacities stack. Your goal is to determine the maximum total cooling capacity that can be achieved from the Chiller to the CPU Cluster using the available network.

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
There are two main paths to transmit coolant from node 1 to node 4:
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
- The first line contains two integers n and m: the number of valves and the number of pipes.
- The next m lines describe the pipes. Each line contains three integers u, v, and c, indicating a one-way pipe from Valve u to Valve v with capacity c.

## Output Format
- Return one integer: the maximum cooling capacity from Valve 1 to Valve n.

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
