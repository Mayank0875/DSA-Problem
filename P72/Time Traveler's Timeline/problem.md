## Title
Time Traveler's Timeline

## Slug
time-travelers-timeline

## Difficulty
Hard

## Description
A time traveler jumps through eras. Starting in the Ancient Era (1), they must reach the Future Era (n). Eras are connected by temporal rifts.

The traveler must start at the Ancient Era (labeled 1) and finish at the Future Era (labeled n). However, to fix anomalies in every time period, the traveler must visit **every single era exactly once** during the journey.

You are given the map of the eras and the directed rifts connecting them. Your task is to calculate the total number of distinct valid paths the traveler can take to complete the timeline correction. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every era exactly once:
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
- The first line contains two integers n and m: the number of eras and the number of rifts.
- The eras are numbered 1, 2, ..., n.
- The next m lines describe the rifts. Each line has two integers a and b, indicating a one-way rift from era a to era b.

## Output Format
- Return one integer: the number of possible timeline correction paths modulo 10^9+7.

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
