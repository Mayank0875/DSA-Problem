## Title
Mining Shaft Support

## Slug
mining-shaft-support

## Difficulty
Medium

## Description
Shaft junctions need reinforcement. Engineers place support beams between adjacent junctions. Each junction supports one beam.

The structure is a tree with n junctions and n-1 tunnels.
A beam is formed between two junctions connected by a tunnel.
However, each junction can be part of at most one beam.

Your task is to calculate the maximum number of beams that can be formed.

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
One optimal set of beams is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 beams.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form beams (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of junctions.
- The next n-1 lines each contain two integers u and v, representing a tunnel between junction u and junction v.

## Output Format
- Return a single integer representing the maximum number of beams.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
