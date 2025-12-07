## Title
Solar Battery Charge

## Slug
solar-battery-charge

## Difficulty
Hard

## Description
Energy flows from solar panels to the main battery bank. The wiring and charge controllers have current limits.

The network consists of n controllers, numbered 1 to n.
1. Controller 1 is the Solar Array.
2. Controller n is the Battery Bank.

There are m one-way wires connecting these controllers. Each wire has a specific capacity, measured in watts, which limits the rate at which energy can flow through it.

Multiple wires can exist between the same two controllers, and their capacities stack. Your goal is to determine the maximum total charging power that can be achieved from the Solar Array to the Battery Bank using the available network.

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
There are two main paths to transmit energy from node 1 to node 4:
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
- The first line contains two integers n and m: the number of controllers and the number of wires.
- The next m lines describe the wires. Each line contains three integers u, v, and c, indicating a one-way wire from Controller u to Controller v with capacity c.

## Output Format
- Return one integer: the maximum charging power from Controller 1 to Controller n.

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
