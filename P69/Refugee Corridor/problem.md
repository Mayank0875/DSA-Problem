## Title
Refugee Corridor

## Slug
refugee-corridor

## Difficulty
Hard

## Description
People are escaping a conflict zone to a border crossing. The safe paths are narrow and can only allow a few people at a time.

The network consists of n shelters, numbered 1 to n.
1. Shelter 1 is the Conflict Zone.
2. Shelter n is the Border.

There are m one-way paths connecting these shelters. Each path has a specific capacity, measured in people per hour, which limits the rate at which refugees can flow through it.

Multiple paths can exist between the same two shelters, and their capacities stack. Your goal is to determine the maximum total escape rate that can be achieved from the Conflict Zone to the Border using the available network.

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
There are two main paths to transmit refugees from node 1 to node 4:
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
- The first line contains two integers n and m: the number of shelters and the number of paths.
- The next m lines describe the paths. Each line contains three integers u, v, and c, indicating a one-way path from Shelter u to Shelter v with capacity c.

## Output Format
- Return one integer: the maximum escape rate from Shelter 1 to Shelter n.

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
