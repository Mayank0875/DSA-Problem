## Title
Subway Connectivity

## Slug
subway-connectivity

## Difficulty
Medium

## Description
A subway system has N stations and one-way tracks. A Zone is a set of stations where passengers can travel between any two stations within the set.

Two stations a and b belong to the same Zone if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of tracks.
In other words, two stations are in the same Zone if they are mutually reachable.

Your task is to: Determine how many Zones exist in total.

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
The stations form two distinct groups where round-trip traversal is possible within each group.
Stations {1, 2, 3} form one Zone.
Path: 1 -> 2 -> 3 -> 1.
Stations {4, 5} form another Zone.
Path: 4 -> 5 -> 4.
Total Zones: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 stations and 1 one-way track.
Track: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Zones.

## Input Format
- The first line contains two integers n and m: the number of stations and tracks.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way track from station a to station b.

## Output Format
- Return one integer: the total number of Zones.

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
