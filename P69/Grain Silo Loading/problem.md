## Title
Grain Silo Loading

## Slug
grain-silo-loading

## Difficulty
Hard

## Description
Grain is moved from the truck unloading pit to the top of the silo. The elevators and belts have capacity limits.

The network consists of n hoppers, numbered 1 to n.
1. Hopper 1 is the Pit.
2. Hopper n is the Silo Top.

There are m one-way elevators connecting these hoppers. Each elevator has a specific capacity, measured in bushels per hour, which limits the rate at which grain can flow through it.

Multiple elevators can exist between the same two hoppers, and their capacities stack. Your goal is to determine the maximum total loading rate that can be achieved from the Pit to the Silo Top using the available network.

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
There are two main paths to transmit grain from node 1 to node 4:
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
- The first line contains two integers n and m: the number of hoppers and the number of elevators.
- The next m lines describe the elevators. Each line contains three integers u, v, and c, indicating a one-way elevator from Hopper u to Hopper v with capacity c.

## Output Format
- Return one integer: the maximum loading rate from Hopper 1 to Hopper n.

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
