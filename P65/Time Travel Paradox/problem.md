## Title
Time Travel Paradox

## Slug
time-travel-paradox

## Difficulty
Medium

## Description
Timelines connect to others via portals. A Paradox Loop is a set of timelines where you can return to your starting timeline.

Two timelines a and b belong to the same Paradox Loop if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of portals.
In other words, two timelines are in the same Paradox Loop if they are mutually reachable.

Your task is to: Determine how many Paradox Loops exist in total.

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
The timelines form two distinct groups where round-trip traversal is possible within each group.
Timelines {1, 2, 3} form one Paradox Loop.
Path: 1 -> 2 -> 3 -> 1.
Timelines {4, 5} form another Paradox Loop.
Path: 4 -> 5 -> 4.
Total Paradox Loops: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 timelines and 1 one-way portal.
Portal: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Paradox Loops.

## Input Format
- The first line contains two integers n and m: the number of timelines and portals.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way portal from timeline a to timeline b.

## Output Format
- Return one integer: the total number of Paradox Loops.

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
