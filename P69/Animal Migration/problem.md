## Title
Animal Migration

## Slug
animal-migration

## Difficulty
Hard

## Description
Herds of wildebeest move from the grazing grounds to the river crossing. The narrow trails limit how many animals can pass.

The network consists of n clearings, numbered 1 to n.
1. Clearing 1 is the Grazing Ground.
2. Clearing n is the River.

There are m one-way trails connecting these clearings. Each trail has a specific capacity, measured in animals per minute, which limits the rate at which animals can flow through it.

Multiple trails can exist between the same two clearings, and their capacities stack. Your goal is to determine the maximum total migration flow that can be achieved from the Grazing Ground to the River using the available network.

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
There are two main paths to transmit animals from node 1 to node 4:
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
- The first line contains two integers n and m: the number of clearings and the number of trails.
- The next m lines describe the trails. Each line contains three integers u, v, and c, indicating a one-way trail from Clearing u to Clearing v with capacity c.

## Output Format
- Return one integer: the maximum migration flow from Clearing 1 to Clearing n.

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
