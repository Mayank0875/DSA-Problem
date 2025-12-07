## Title
Sewer Inspection

## Slug
sewer-inspection

## Difficulty
Hard

## Description
A worker inspects the sewers. Starting at Manhole 1, they must reach the Treatment Plant (n). Junctions are connected by pipes.

The worker must start at the Manhole 1 (labeled 1) and finish at the Treatment Plant (labeled n). However, to verify the flow at every junction, the worker must visit **every single junction exactly once** during the journey.

You are given the map of the junctions and the directed pipes connecting them. Your task is to calculate the total number of distinct valid paths the worker can take to complete the inspection. As the number of paths can be very large, print the answer modulo 1000000007.

## Examples

### 1

#### Input
4 6
1 2
1 3
2 3
3 2
2 4
3 4

#### Output
2

#### Explanation
There are two possible paths that visit every junction exactly once:
1 -> 2 -> 3 -> 4
1 -> 3 -> 2 -> 4

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
The only valid path is 1 -> 2.

## Input Format
- The first line contains two integers n and m: the number of junctions and the number of pipes.
- The junctions are numbered 1, 2, ..., n.
- The next m lines describe the pipes. Each line has two integers a and b, indicating a one-way pipe from junction a to junction b.

## Output Format
- Return one integer: the number of possible inspection paths modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 20
- 1 ≤ m ≤ n * n
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
