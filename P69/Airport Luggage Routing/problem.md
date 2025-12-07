## Title
Airport Luggage Routing

## Slug
airport-luggage-routing

## Difficulty
Hard

## Description
Luggage moves from the check-in counter to the plane cargo hold. The belt system consists of various junctions with capacity limits.

The network consists of n junctions, numbered 1 to n.
1. Junction 1 is the Check-in.
2. Junction n is the Plane.

There are m one-way belts connecting these junctions. Each belt has a specific capacity, measured in bags per minute, which limits the rate at which luggage can flow through it.

Multiple belts can exist between the same two junctions, and their capacities stack. Your goal is to determine the maximum total baggage handling that can be achieved from the Check-in to the Plane using the available network.

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
There are two main paths to transmit luggage from node 1 to node 4:
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
- The first line contains two integers n and m: the number of junctions and the number of belts.
- The next m lines describe the belts. Each line contains three integers u, v, and c, indicating a one-way belt from Junction u to Junction v with capacity c.

## Output Format
- Return one integer: the maximum baggage handling from Junction 1 to Junction n.

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
