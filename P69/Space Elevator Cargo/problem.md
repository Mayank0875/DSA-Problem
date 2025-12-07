## Title
Space Elevator Cargo

## Slug
space-elevator-cargo

## Difficulty
Hard

## Description
Cargo pods travel up the tether from Earth to the Orbital Station. The climber tracks have weight throughput limits.

The network consists of n platforms, numbered 1 to n.
1. Platform 1 is the Earth Port.
2. Platform n is the Orbital Station.

There are m one-way tracks connecting these platforms. Each track has a specific capacity, measured in tons per hour, which limits the rate at which cargo can flow through it.

Multiple tracks can exist between the same two platforms, and their capacities stack. Your goal is to determine the maximum total lift capacity that can be achieved from the Earth Port to the Orbital Station using the available network.

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
There are two main paths to transmit cargo from node 1 to node 4:
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
- The first line contains two integers n and m: the number of platforms and the number of tracks.
- The next m lines describe the tracks. Each line contains three integers u, v, and c, indicating a one-way track from Platform u to Platform v with capacity c.

## Output Format
- Return one integer: the maximum lift capacity from Platform 1 to Platform n.

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
