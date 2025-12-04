## Title
Traffic Zones

## Slug
traffic-zones

## Difficulty
Medium

## Description
A city has N intersections connected by one-way streets. A Traffic Zone is a set of intersections where a car can drive from any intersection to any other within the zone.

Two intersections a and b belong to the same Traffic Zone if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of streets.
In other words, two intersections are in the same Traffic Zone if they are mutually reachable.

Your task is to: Determine how many Traffic Zones exist in total.

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
The intersections form two distinct groups where round-trip traversal is possible within each group.
Intersections {1, 2, 3} form one Traffic Zone.
Path: 1 -> 2 -> 3 -> 1.
Intersections {4, 5} form another Traffic Zone.
Path: 4 -> 5 -> 4.
Total Traffic Zones: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 intersections and 1 one-way street.
Street: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Traffic Zones.

## Input Format
- The first line contains two integers n and m: the number of intersections and streets.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way street from intersection a to intersection b.

## Output Format
- Return one integer: the total number of Traffic Zones.

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
