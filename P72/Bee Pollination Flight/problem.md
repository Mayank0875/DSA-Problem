## Title
Bee Pollination Flight

## Slug
bee-pollination-flight

## Difficulty
Hard

## Description
A robotic bee pollinates a greenhouse. It starts at Flower 1 and ends at the Hive (n). Flowers are connected by flight paths.

The bee must start at the First Flower (labeled 1) and finish at the Hive (labeled n). However, to ensure every flower is pollinated, the bee must visit **every single flower exactly once** during the journey.

You are given the map of the flowers and the directed flight paths connecting them. Your task is to calculate the total number of distinct valid paths the bee can take to complete the flight. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every flower exactly once:
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
- The first line contains two integers n and m: the number of flowers and the number of flight paths.
- The flowers are numbered 1, 2, ..., n.
- The next m lines describe the flight paths. Each line has two integers a and b, indicating a one-way flight path from flower a to flower b.

## Output Format
- Return one integer: the number of possible flight paths modulo 10^9+7.

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
