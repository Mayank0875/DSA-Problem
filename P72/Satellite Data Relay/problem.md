## Title
Satellite Data Relay

## Slug
satellite-data-relay

## Difficulty
Hard

## Description
Data is beamed across space. Starting at Satellite 1, it must reach Earth Station (n). Satellites are connected by laser beams.

The data must start at the Satellite 1 (labeled 1) and finish at the Earth Station (labeled n). However, to sync clocks with every satellite in the constellation, the data must visit **every single satellite exactly once** during the journey.

You are given the map of the satellites and the directed beams connecting them. Your task is to calculate the total number of distinct valid paths the data can take to complete the relay. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every satellite exactly once:
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
- The first line contains two integers n and m: the number of satellites and the number of beams.
- The satellites are numbered 1, 2, ..., n.
- The next m lines describe the beams. Each line has two integers a and b, indicating a one-way beam from satellite a to satellite b.

## Output Format
- Return one integer: the number of possible relay paths modulo 10^9+7.

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
