## Title
Ski Resort Lift Network

## Slug
ski-resort-lift-network

## Difficulty
Hard

## Description
Skiers move from the base lodge to the summit. The chairlifts and gondolas have hourly passenger capacities.

The network consists of n towers, numbered 1 to n.
1. Lift Tower 1 is the Base Lodge.
2. Lift Tower n is the Summit.

There are m one-way lifts connecting these towers. Each lift has a specific capacity, measured in skiers per hour, which limits the rate at which skiers can flow through it.

Multiple lifts can exist between the same two towers, and their capacities stack. Your goal is to determine the maximum total uphill capacity that can be achieved from the Base Lodge to the Summit using the available network.

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
There are two main paths to transmit skiers from node 1 to node 4:
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
- The first line contains two integers n and m: the number of towers and the number of lifts.
- The next m lines describe the lifts. Each line contains three integers u, v, and c, indicating a one-way lift from Lift Tower u to Lift Tower v with capacity c.

## Output Format
- Return one integer: the maximum uphill capacity from Lift Tower 1 to Lift Tower n.

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
