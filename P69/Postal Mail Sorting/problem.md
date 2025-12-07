## Title
Postal Mail Sorting

## Slug
postal-mail-sorting

## Difficulty
Hard

## Description
Letters move from the drop box to the local delivery truck. The sorting machines and chutes have throughput limits.

The network consists of n sorters, numbered 1 to n.
1. Sorter 1 is the Drop Box.
2. Sorter n is the Truck.

There are m one-way chutes connecting these sorters. Each chute has a specific capacity, measured in letters per second, which limits the rate at which mail can flow through it.

Multiple chutes can exist between the same two sorters, and their capacities stack. Your goal is to determine the maximum total sorting speed that can be achieved from the Drop Box to the Truck using the available network.

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
There are two main paths to transmit mail from node 1 to node 4:
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
- The first line contains two integers n and m: the number of sorters and the number of chutes.
- The next m lines describe the chutes. Each line contains three integers u, v, and c, indicating a one-way chute from Sorter u to Sorter v with capacity c.

## Output Format
- Return one integer: the maximum sorting speed from Sorter 1 to Sorter n.

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
