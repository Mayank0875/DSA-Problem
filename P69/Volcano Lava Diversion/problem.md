## Title
Volcano Lava Diversion

## Slug
volcano-lava-diversion

## Difficulty
Hard

## Description
Engineers dig trenches to divert lava from a vent to the ocean. Each trench can only handle a certain volume of flow.

The network consists of n junctions, numbered 1 to n.
1. Junction 1 is the Volcano Vent.
2. Junction n is the Ocean.

There are m one-way trenches connecting these junctions. Each trench has a specific capacity, measured in cubic meters per second, which limits the rate at which lava can flow through it.

Multiple trenches can exist between the same two junctions, and their capacities stack. Your goal is to determine the maximum total diversion rate that can be achieved from the Volcano Vent to the Ocean using the available network.

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
There are two main paths to transmit lava from node 1 to node 4:
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
- The first line contains two integers n and m: the number of junctions and the number of trenches.
- The next m lines describe the trenches. Each line contains three integers u, v, and c, indicating a one-way trench from Junction u to Junction v with capacity c.

## Output Format
- Return one integer: the maximum diversion rate from Junction 1 to Junction n.

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
