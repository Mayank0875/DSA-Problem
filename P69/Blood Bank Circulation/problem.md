## Title
Blood Bank Circulation

## Slug
blood-bank-circulation

## Difficulty
Hard

## Description
In a biological simulation, blood must flow from the heart to a specific organ. The arteries and veins have flow volume limits.

The network consists of n vessels, numbered 1 to n.
1. Vessel Node 1 is the Heart.
2. Vessel Node n is the Organ.

There are m one-way arteries connecting these vessels. Each artery has a specific capacity, measured in milliliters per second, which limits the rate at which blood can flow through it.

Multiple arteries can exist between the same two vessels, and their capacities stack. Your goal is to determine the maximum total blood flow that can be achieved from the Heart to the Organ using the available network.

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
There are two main paths to transmit blood from node 1 to node 4:
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
- The first line contains two integers n and m: the number of vessels and the number of arteries.
- The next m lines describe the arteries. Each line contains three integers u, v, and c, indicating a one-way artery from Vessel Node u to Vessel Node v with capacity c.

## Output Format
- Return one integer: the maximum blood flow from Vessel Node 1 to Vessel Node n.

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
