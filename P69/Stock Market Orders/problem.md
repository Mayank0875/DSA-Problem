## Title
Stock Market Orders

## Slug
stock-market-orders

## Difficulty
Hard

## Description
Buy orders must be matched with sell orders through a series of brokers. Each broker has a limit on the volume they can handle.

The network consists of n brokers, numbered 1 to n.
1. Broker 1 is the Buyer.
2. Broker n is the Seller.

There are m one-way connections connecting these brokers. Each connection has a specific capacity, measured in shares per second, which limits the rate at which stocks can flow through it.

Multiple connections can exist between the same two brokers, and their capacities stack. Your goal is to determine the maximum total trading volume that can be achieved from the Buyer to the Seller using the available network.

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
There are two main paths to transmit stocks from node 1 to node 4:
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
- The first line contains two integers n and m: the number of brokers and the number of connections.
- The next m lines describe the connections. Each line contains three integers u, v, and c, indicating a one-way connection from Broker u to Broker v with capacity c.

## Output Format
- Return one integer: the maximum trading volume from Broker 1 to Broker n.

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
