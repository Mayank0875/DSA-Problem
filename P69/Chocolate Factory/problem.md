## Title
Chocolate Factory

## Slug
chocolate-factory

## Difficulty
Hard

## Description
Liquid chocolate flows from the melting tank to the molding machine. The heated pipes have flow limits to prevent clogging.

The network consists of n pumps, numbered 1 to n.
1. Pump 1 is the Melting Tank.
2. Pump n is the Molding Machine.

There are m one-way pipes connecting these pumps. Each pipe has a specific capacity, measured in liters per minute, which limits the rate at which chocolate can flow through it.

Multiple pipes can exist between the same two pumps, and their capacities stack. Your goal is to determine the maximum total production flow that can be achieved from the Melting Tank to the Molding Machine using the available network.

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
There are two main paths to transmit chocolate from node 1 to node 4:
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
- The first line contains two integers n and m: the number of pumps and the number of pipes.
- The next m lines describe the pipes. Each line contains three integers u, v, and c, indicating a one-way pipe from Pump u to Pump v with capacity c.

## Output Format
- Return one integer: the maximum production flow from Pump 1 to Pump n.

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
