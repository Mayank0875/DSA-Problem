## Title
Microchip Data Bus

## Slug
microchip-data-bus

## Difficulty
Hard

## Description
Data signals move from the CPU to the RAM. The bus lines on the motherboard have bandwidth limits.

The network consists of n chips, numbered 1 to n.
1. Chip 1 is the CPU.
2. Chip n is the RAM.

There are m one-way traces connecting these chips. Each trace has a specific capacity, measured in bits per cycle, which limits the rate at which data can flow through it.

Multiple traces can exist between the same two chips, and their capacities stack. Your goal is to determine the maximum total data transfer that can be achieved from the CPU to the RAM using the available network.

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
- The first line contains two integers n and m: the number of chips and the number of traces.
- The next m lines describe the traces. Each line contains three integers u, v, and c, indicating a one-way trace from Chip u to Chip v with capacity c.

## Output Format
- Return one integer: the maximum data transfer from Chip 1 to Chip n.

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
