## Title
Train Cargo Logistics

## Slug
train-cargo-logistics

## Difficulty
Hard

## Description
Coal moves from mines to the power plant via a rail network. Each track segment has a maximum daily tonnage limit.

The network consists of n yards, numbered 1 to n.
1. Rail Yard 1 is the Mine.
2. Rail Yard n is the Power Plant.

There are m one-way tracks connecting these yards. Each track has a specific capacity, measured in tons per day, which limits the rate at which coal can flow through it.

Multiple tracks can exist between the same two yards, and their capacities stack. Your goal is to determine the maximum total freight capacity that can be achieved from the Mine to the Power Plant using the available network.

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
There are two main paths to transmit coal from node 1 to node 4:
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
- The first line contains two integers n and m: the number of yards and the number of tracks.
- The next m lines describe the tracks. Each line contains three integers u, v, and c, indicating a one-way track from Rail Yard u to Rail Yard v with capacity c.

## Output Format
- Return one integer: the maximum freight capacity from Rail Yard 1 to Rail Yard n.

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
