## Title
Glacier Meltwater

## Slug
glacier-meltwater

## Difficulty
Hard

## Description
Meltwater flows from the glacier peak to the lake below. The crevices and channels in the ice restrict the flow volume.

The network consists of n pools, numbered 1 to n.
1. Pool 1 is the Peak.
2. Pool n is the Lake.

There are m one-way channels connecting these pools. Each channel has a specific capacity, measured in liters per second, which limits the rate at which water can flow through it.

Multiple channels can exist between the same two pools, and their capacities stack. Your goal is to determine the maximum total melt rate that can be achieved from the Peak to the Lake using the available network.

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
- The first line contains two integers n and m: the number of pools and the number of channels.
- The next m lines describe the channels. Each line contains three integers u, v, and c, indicating a one-way channel from Pool u to Pool v with capacity c.

## Output Format
- Return one integer: the maximum melt rate from Pool 1 to Pool n.

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
