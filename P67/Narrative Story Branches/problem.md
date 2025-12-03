## Title
Narrative Story Branches

## Slug
narrative-story-branches

## Difficulty
Medium

## Description
An interactive novel starts at Chapter 1. The reader makes choices that lead to different chapters, eventually concluding at Ending n.

There are n chapters numbered from 1 to n.
    1. Chapter 1 is the starting point.
    2. Chapter n is the destination.

Between some chapters, there are one-way plot choices that allow movement from u to v. The system contains no loops (directed acyclic graph), meaning you can only move forward towards the goal.

Your task is to find the total number of distinct ways/paths to travel from Chapter 1 to Chapter n. Since the answer can be very large, return the count modulo 1000000007.

## Examples

### 1

#### Input
4 5
1 2
2 4
1 3
3 4
1 4

#### Output
3

#### Explanation
There are 3 distinct paths:
1 -> 2 -> 4
1 -> 3 -> 4
1 -> 4

### 2

#### Input
4 5
1 2
3 4
2 3
1 3
2 4

#### Output
3

#### Explanation
There are 3 distinct paths:
1 -> 2 -> 3 -> 4
1 -> 2 -> 4
1 -> 3 -> 4

## Input Format
- The first line contains two integers n and m: the number of chapters and the number of plot choices.
- The next m lines each contain two integers u and v, representing a one-way choice from u to v.

## Output Format
- Return a single integer: the number of ways to travel from 1 to n, modulo (1e9 + 7).

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
