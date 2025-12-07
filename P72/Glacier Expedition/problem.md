## Title
Glacier Expedition

## Slug
glacier-expedition

## Difficulty
Hard

## Description
Scientists cross a glacier. Starting at the Edge (1), they must reach the Research Station (n). Ice plateaus are connected by ice bridges.

The team must start at the Edge (labeled 1) and finish at the Research Station (labeled n). However, to take samples from every plateau, the team must visit **every single plateau exactly once** during the journey.

You are given the map of the plateaus and the directed bridges connecting them. Your task is to calculate the total number of distinct valid paths the team can take to complete the crossing. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every plateau exactly once:
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
- The first line contains two integers n and m: the number of plateaus and the number of bridges.
- The plateaus are numbered 1, 2, ..., n.
- The next m lines describe the bridges. Each line has two integers a and b, indicating a one-way bridge from plateau a to plateau b.

## Output Format
- Return one integer: the number of possible crossing paths modulo 10^9+7.

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
