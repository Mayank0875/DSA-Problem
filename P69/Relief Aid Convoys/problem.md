## Title
Relief Aid Convoys

## Slug
relief-aid-convoys

## Difficulty
Hard

## Description
Food supplies must be moved from the airport to a refugee camp. The roads are damaged and can only support a limited number of trucks.

The network consists of n towns, numbered 1 to n.
1. Town 1 is the Airport.
2. Town n is the Camp.

There are m one-way roads connecting these towns. Each road has a specific capacity, measured in trucks per day, which limits the rate at which trucks can flow through it.

Multiple roads can exist between the same two towns, and their capacities stack. Your goal is to determine the maximum total aid delivery that can be achieved from the Airport to the Camp using the available network.

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
There are two main paths to transmit trucks from node 1 to node 4:
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
- The first line contains two integers n and m: the number of towns and the number of roads.
- The next m lines describe the roads. Each line contains three integers u, v, and c, indicating a one-way road from Town u to Town v with capacity c.

## Output Format
- Return one integer: the maximum aid delivery from Town 1 to Town n.

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
