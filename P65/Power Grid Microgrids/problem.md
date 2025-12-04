## Title
Power Grid Microgrids

## Slug
power-grid-microgrids

## Difficulty
Medium

## Description
Power stations connect via directional lines. A Microgrid is a subset of stations that can share power cyclically.

Two stations a and b belong to the same Microgrid if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of lines.
In other words, two stations are in the same Microgrid if they are mutually reachable.

Your task is to: Determine how many Microgrids exist in total.

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
Stations {1, 2, 3} form one Microgrid.
Path: 1 -> 2 -> 3 -> 1.
Stations {4, 5} form another Microgrid.
Path: 4 -> 5 -> 4.
Total Microgrids: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 stations and 1 one-way line.
Line: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Microgrids.

## Input Format
- The first line contains two integers n and m: the number of stations and lines.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way line from station a to station b.

## Output Format
- Return one integer: the total number of Microgrids.

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
