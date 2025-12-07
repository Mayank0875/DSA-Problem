## Title
Bank Money Transfer

## Slug
bank-money-transfer

## Difficulty
Hard

## Description
Funds are transferred from a sender account to a receiver account through a network of intermediary banks with transaction limits.

The network consists of n banks, numbered 1 to n.
1. Bank 1 is the Sender Bank.
2. Bank n is the Receiver Bank.

There are m one-way channels connecting these banks. Each channel has a specific capacity, measured in dollars per hour, which limits the rate at which money can flow through it.

Multiple channels can exist between the same two banks, and their capacities stack. Your goal is to determine the maximum total transaction volume that can be achieved from the Sender Bank to the Receiver Bank using the available network.

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
There are two main paths to transmit money from node 1 to node 4:
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
- The first line contains two integers n and m: the number of banks and the number of channels.
- The next m lines describe the channels. Each line contains three integers u, v, and c, indicating a one-way channel from Bank u to Bank v with capacity c.

## Output Format
- Return one integer: the maximum transaction volume from Bank 1 to Bank n.

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
