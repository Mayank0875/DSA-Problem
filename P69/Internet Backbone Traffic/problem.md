## Title
Internet Backbone Traffic

## Slug
internet-backbone-traffic

## Difficulty
Hard

## Description
An ISP needs to route data traffic from a regional server to a home router. The fiber optic cables have bandwidth limits.

The network consists of n routers, numbered 1 to n.
1. Router 1 is the Server.
2. Router n is the Home.

There are m one-way cables connecting these routers. Each cable has a specific capacity, measured in gigabits per second, which limits the rate at which data can flow through it.

Multiple cables can exist between the same two routers, and their capacities stack. Your goal is to determine the maximum total bandwidth that can be achieved from the Server to the Home using the available network.

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
There are two main paths to transmit data from node 1 to node 4:
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
- The first line contains two integers n and m: the number of routers and the number of cables.
- The next m lines describe the cables. Each line contains three integers u, v, and c, indicating a one-way cable from Router u to Router v with capacity c.

## Output Format
- Return one integer: the maximum bandwidth from Router 1 to Router n.

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
