## Title
Ant Colony Foraging

## Slug
ant-colony-foraging

## Difficulty
Hard

## Description
An ant looks for food. Starting at the Nest (1), it must reach the Surface (n). Chambers are connected by tunnels.

The ant must start at the Nest (labeled 1) and finish at the Surface (labeled n). However, to leave pheromones in every chamber, the ant must visit **every single chamber exactly once** during the journey.

You are given the map of the chambers and the directed tunnels connecting them. Your task is to calculate the total number of distinct valid paths the ant can take to complete the foraging run. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every chamber exactly once:
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
- The first line contains two integers n and m: the number of chambers and the number of tunnels.
- The chambers are numbered 1, 2, ..., n.
- The next m lines describe the tunnels. Each line has two integers a and b, indicating a one-way tunnel from chamber a to chamber b.

## Output Format
- Return one integer: the number of possible foraging run paths modulo 10^9+7.

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
