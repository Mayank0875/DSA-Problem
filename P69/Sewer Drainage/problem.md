## Title
Sewer Drainage

## Slug
sewer-drainage

## Difficulty
Hard

## Description
Stormwater flows from street drains to the treatment plant. The sewer pipes vary in diameter and capacity.

The network consists of n manholes, numbered 1 to n.
1. Manhole 1 is the Street Drain.
2. Manhole n is the Treatment Plant.

There are m one-way pipes connecting these manholes. Each pipe has a specific capacity, measured in gallons per minute, which limits the rate at which water can flow through it.

Multiple pipes can exist between the same two manholes, and their capacities stack. Your goal is to determine the maximum total drainage that can be achieved from the Street Drain to the Treatment Plant using the available network.

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
- The first line contains two integers n and m: the number of manholes and the number of pipes.
- The next m lines describe the pipes. Each line contains three integers u, v, and c, indicating a one-way pipe from Manhole u to Manhole v with capacity c.

## Output Format
- Return one integer: the maximum drainage from Manhole 1 to Manhole n.

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
