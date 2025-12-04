## Title
Flight Networks

## Slug
flight-networks

## Difficulty
Medium

## Description
Airports have one-way flight legs. A Region is a set of airports where round trips are possible between any two.

Two airports a and b belong to the same Region if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of flights.
In other words, two airports are in the same Region if they are mutually reachable.

Your task is to: Determine how many Regions exist in total.

## Examples

### 1

#### Input
5 6
1 2
2 3
3 1
3 4
4 5
5 4

#### Output
2

#### Explanation
The airports form two distinct groups where round-trip traversal is possible within each group.
Airports {1, 2, 3} form one Region.
Path: 1 -> 2 -> 3 -> 1.
Airports {4, 5} form another Region.
Path: 4 -> 5 -> 4.
Total Regions: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 airports and 1 one-way flight.
Flight: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Regions.

## Input Format
- The first line contains two integers n and m: the number of airports and flights.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way flight from airport a to airport b.

## Output Format
- Return one integer: the total number of Regions.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search
