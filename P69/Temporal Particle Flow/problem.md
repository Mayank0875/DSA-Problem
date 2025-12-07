## Title
Temporal Particle Flow

## Slug
temporal-particle-flow

## Difficulty
Hard

## Description
In a sci-fi accelerator, chronon particles flow from the past generator to the future receiver. The containment fields have flux limits.

The network consists of n fields, numbered 1 to n.
1. Field Generator 1 is the Past.
2. Field Generator n is the Future.

There are m one-way conduits connecting these fields. Each conduit has a specific capacity, measured in chronons per nanosecond, which limits the rate at which particles can flow through it.

Multiple conduits can exist between the same two fields, and their capacities stack. Your goal is to determine the maximum total time flow that can be achieved from the Past to the Future using the available network.

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
There are two main paths to transmit particles from node 1 to node 4:
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
- The first line contains two integers n and m: the number of fields and the number of conduits.
- The next m lines describe the conduits. Each line contains three integers u, v, and c, indicating a one-way conduit from Field Generator u to Field Generator v with capacity c.

## Output Format
- Return one integer: the maximum time flow from Field Generator 1 to Field Generator n.

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
