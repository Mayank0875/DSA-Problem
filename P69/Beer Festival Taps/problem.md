## Title
Beer Festival Taps

## Slug
beer-festival-taps

## Difficulty
Hard

## Description
Beer flows from the main keg room to the festival tap wall. The tubing system has restrictions on flow rate.

The network consists of n connectors, numbered 1 to n.
1. Connector 1 is the Keg Room.
2. Connector n is the Tap Wall.

There are m one-way tubes connecting these connectors. Each tube has a specific capacity, measured in pints per minute, which limits the rate at which beer can flow through it.

Multiple tubes can exist between the same two connectors, and their capacities stack. Your goal is to determine the maximum total pouring rate that can be achieved from the Keg Room to the Tap Wall using the available network.

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
There are two main paths to transmit beer from node 1 to node 4:
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
- The first line contains two integers n and m: the number of connectors and the number of tubes.
- The next m lines describe the tubes. Each line contains three integers u, v, and c, indicating a one-way tube from Connector u to Connector v with capacity c.

## Output Format
- Return one integer: the maximum pouring rate from Connector 1 to Connector n.

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
