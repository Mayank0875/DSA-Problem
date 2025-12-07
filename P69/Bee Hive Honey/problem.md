## Title
Bee Hive Honey

## Slug
bee-hive-honey

## Difficulty
Hard

## Description
Bees move nectar from flowers to the honeycomb. The hive corridors allow only a certain number of bees to pass.

The network consists of n chambers, numbered 1 to n.
1. Chamber 1 is the Entrance.
2. Chamber n is the Honeycomb.

There are m one-way corridors connecting these chambers. Each corridor has a specific capacity, measured in drops per minute, which limits the rate at which nectar can flow through it.

Multiple corridors can exist between the same two chambers, and their capacities stack. Your goal is to determine the maximum total honey production that can be achieved from the Entrance to the Honeycomb using the available network.

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
There are two main paths to transmit nectar from node 1 to node 4:
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
- The first line contains two integers n and m: the number of chambers and the number of corridors.
- The next m lines describe the corridors. Each line contains three integers u, v, and c, indicating a one-way corridor from Chamber u to Chamber v with capacity c.

## Output Format
- Return one integer: the maximum honey production from Chamber 1 to Chamber n.

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
