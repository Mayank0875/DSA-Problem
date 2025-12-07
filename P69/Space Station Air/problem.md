## Title
Space Station Air

## Slug
space-station-air

## Difficulty
Hard

## Description
Oxygen is pumped from the generation module to the crew quarters. The ventilation ducts have airflow limits.

The network consists of n vents, numbered 1 to n.
1. Vent 1 is the Generator.
2. Vent n is the Quarters.

There are m one-way ducts connecting these vents. Each duct has a specific capacity, measured in cubic feet per minute, which limits the rate at which air can flow through it.

Multiple ducts can exist between the same two vents, and their capacities stack. Your goal is to determine the maximum total airflow that can be achieved from the Generator to the Quarters using the available network.

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
There are two main paths to transmit air from node 1 to node 4:
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
- The first line contains two integers n and m: the number of vents and the number of ducts.
- The next m lines describe the ducts. Each line contains three integers u, v, and c, indicating a one-way duct from Vent u to Vent v with capacity c.

## Output Format
- Return one integer: the maximum airflow from Vent 1 to Vent n.

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
