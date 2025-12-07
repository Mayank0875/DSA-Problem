## Title
Aquarium Filter System

## Slug
aquarium-filter-system

## Difficulty
Hard

## Description
Water cycles from the main tank through filters and back. The pumps and tubing determine the flow rate.

The network consists of n filters, numbered 1 to n.
1. Filter 1 is the Tank Drain.
2. Filter n is the Tank Return.

There are m one-way tubes connecting these filters. Each tube has a specific capacity, measured in liters per hour, which limits the rate at which water can flow through it.

Multiple tubes can exist between the same two filters, and their capacities stack. Your goal is to determine the maximum total filtration rate that can be achieved from the Tank Drain to the Tank Return using the available network.

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
There are two main paths to transmit water from node 1 to node 4:
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
- The first line contains two integers n and m: the number of filters and the number of tubes.
- The next m lines describe the tubes. Each line contains three integers u, v, and c, indicating a one-way tube from Filter u to Filter v with capacity c.

## Output Format
- Return one integer: the maximum filtration rate from Filter 1 to Filter n.

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
