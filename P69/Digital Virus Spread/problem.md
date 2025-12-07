## Title
Digital Virus Spread

## Slug
digital-virus-spread

## Difficulty
Hard

## Description
A simulation tracks malware spreading from an infected server to a target network. The connection speeds limit the infection rate.

The network consists of n computers, numbered 1 to n.
1. Computer 1 is the Infected Server.
2. Computer n is the Target Network.

There are m one-way connections connecting these computers. Each connection has a specific capacity, measured in packets per second, which limits the rate at which malware can flow through it.

Multiple connections can exist between the same two computers, and their capacities stack. Your goal is to determine the maximum total infection rate that can be achieved from the Infected Server to the Target Network using the available network.

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
There are two main paths to transmit malware from node 1 to node 4:
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
- The first line contains two integers n and m: the number of computers and the number of connections.
- The next m lines describe the connections. Each line contains three integers u, v, and c, indicating a one-way connection from Computer u to Computer v with capacity c.

## Output Format
- Return one integer: the maximum infection rate from Computer 1 to Computer n.

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
