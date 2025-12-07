## Title
Firefighter Hoses

## Slug
firefighter-hoses

## Difficulty
Hard

## Description
Water is pumped from a hydrant to the fire engine and then to the nozzle. Splitters and hoses limit the flow.

The network consists of n splitters, numbered 1 to n.
1. Splitter 1 is the Hydrant.
2. Splitter n is the Nozzle.

There are m one-way hoses connecting these splitters. Each hose has a specific capacity, measured in gallons per minute, which limits the rate at which water can flow through it.

Multiple hoses can exist between the same two splitters, and their capacities stack. Your goal is to determine the maximum total extinguishing power that can be achieved from the Hydrant to the Nozzle using the available network.

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
There are two main paths to transmit water from node 1 to node 4:
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
- The first line contains two integers n and m: the number of splitters and the number of hoses.
- The next m lines describe the hoses. Each line contains three integers u, v, and c, indicating a one-way hose from Splitter u to Splitter v with capacity c.

## Output Format
- Return one integer: the maximum extinguishing power from Splitter 1 to Splitter n.

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
