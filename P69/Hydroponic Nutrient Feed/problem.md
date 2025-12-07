## Title
Hydroponic Nutrient Feed

## Slug
hydroponic-nutrient-feed

## Difficulty
Hard

## Description
Nutrient solution flows from the reservoir to the plant roots. The tubing network distributes liquid with specific flow caps.

The network consists of n valves, numbered 1 to n.
1. Valve 1 is the Reservoir.
2. Valve n is the Plants.

There are m one-way tubes connecting these valves. Each tube has a specific capacity, measured in liters per hour, which limits the rate at which nutrients can flow through it.

Multiple tubes can exist between the same two valves, and their capacities stack. Your goal is to determine the maximum total feeding rate that can be achieved from the Reservoir to the Plants using the available network.

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
There are two main paths to transmit nutrients from node 1 to node 4:
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
- The first line contains two integers n and m: the number of valves and the number of tubes.
- The next m lines describe the tubes. Each line contains three integers u, v, and c, indicating a one-way tube from Valve u to Valve v with capacity c.

## Output Format
- Return one integer: the maximum feeding rate from Valve 1 to Valve n.

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
