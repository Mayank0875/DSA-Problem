## Title
Pipeline Valve Test

## Slug
pipeline-valve-test

## Difficulty
Medium

## Description
Valves in a pipeline network need testing. Engineers isolate segments between two adjacent valves. Each valve can be part of only one isolation test.

The structure is a tree with n valves and n-1 pipes.
A test segment is formed between two valves connected by a pipe.
However, each valve can be part of at most one test segment.

Your task is to calculate the maximum number of test segments that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of test segments is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 test segments.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form test segments (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of valves.
- The next n-1 lines each contain two integers u and v, representing a pipe between valve u and valve v.

## Output Format
- Return a single integer representing the maximum number of test segments.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
