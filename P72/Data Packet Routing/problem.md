## Title
Data Packet Routing

## Slug
data-packet-routing

## Difficulty
Hard

## Description
A specialized data packet travels through a server cluster. It starts at Server 1 and targets Server n. The servers are linked by unidirectional fiber cables.

The packet must start at the Source Server (labeled 1) and finish at the Destination Server (labeled n). However, to update the firmware on every server in the cluster, the packet must visit **every single server exactly once** during the journey.

You are given the map of the servers and the directed cables connecting them. Your task is to calculate the total number of distinct valid paths the packet can take to complete the routing. As the number of paths can be very large, print the answer modulo 1000000007.

## Examples

### 1

#### Input
4 6
1 2
1 3
2 3
3 2
2 4
3 4

#### Output
2

#### Explanation
There are two possible paths that visit every server exactly once:
1 -> 2 -> 3 -> 4
1 -> 3 -> 2 -> 4

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
The only valid path is 1 -> 2.

## Input Format
- The first line contains two integers n and m: the number of servers and the number of cables.
- The servers are numbered 1, 2, ..., n.
- The next m lines describe the cables. Each line has two integers a and b, indicating a one-way cable from server a to server b.

## Output Format
- Return one integer: the number of possible routing paths modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 20
- 1 ≤ m ≤ n * n
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
