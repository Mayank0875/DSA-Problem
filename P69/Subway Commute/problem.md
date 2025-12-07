## Title
Subway Commute

## Slug
subway-commute

## Difficulty
Hard

## Description
Commuters travel from the suburbs to the city center. The train lines and transfer stations have capacity limits.

The network consists of n stations, numbered 1 to n.
1. Station 1 is the Suburb.
2. Station n is the City Center.

There are m one-way lines connecting these stations. Each line has a specific capacity, measured in passengers per hour, which limits the rate at which commuters can flow through it.

Multiple lines can exist between the same two stations, and their capacities stack. Your goal is to determine the maximum total transit capacity that can be achieved from the Suburb to the City Center using the available network.

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
There are two main paths to transmit commuters from node 1 to node 4:
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
- The first line contains two integers n and m: the number of stations and the number of lines.
- The next m lines describe the lines. Each line contains three integers u, v, and c, indicating a one-way line from Station u to Station v with capacity c.

## Output Format
- Return one integer: the maximum transit capacity from Station 1 to Station n.

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
