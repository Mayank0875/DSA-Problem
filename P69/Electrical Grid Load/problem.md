## Title
Electrical Grid Load

## Slug
electrical-grid-load

## Difficulty
Hard

## Description
Power must be transmitted from a nuclear plant to a metropolis. The transmission lines have maximum amperage ratings.

The network consists of n substations, numbered 1 to n.
1. Substation 1 is the Power Plant.
2. Substation n is the Metropolis.

There are m one-way transmission lines connecting these substations. Each line has a specific capacity, measured in megawatts, which limits the rate at which electricity can flow through it.

Multiple transmission lines can exist between the same two substations, and their capacities stack. Your goal is to determine the maximum total power transmission that can be achieved from the Power Plant to the Metropolis using the available network.

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
There are two main paths to transmit electricity from node 1 to node 4:
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
- The first line contains two integers n and m: the number of substations and the number of transmission lines.
- The next m lines describe the transmission lines. Each line contains three integers u, v, and c, indicating a one-way line from Substation u to Substation v with capacity c.

## Output Format
- Return one integer: the maximum power transmission from Substation 1 to Substation n.

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
