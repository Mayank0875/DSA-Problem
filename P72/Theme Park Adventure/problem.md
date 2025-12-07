## Title
Theme Park Adventure

## Slug
theme-park-adventure

## Difficulty
Hard

## Description
A guest wants to ride everything. Starting at the Entrance (1), they must reach the Exit (n). Rides are connected by paths.

The guest must start at the Entrance (labeled 1) and finish at the Exit (labeled n). However, to experience every ride exactly once, the guest must visit **every single ride exactly once** during the journey.

You are given the map of the rides and the directed paths connecting them. Your task is to calculate the total number of distinct valid paths the guest can take to complete the adventure. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every ride exactly once:
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
- The first line contains two integers n and m: the number of rides and the number of paths.
- The rides are numbered 1, 2, ..., n.
- The next m lines describe the paths. Each line has two integers a and b, indicating a one-way path from ride a to ride b.

## Output Format
- Return one integer: the number of possible adventure paths modulo 10^9+7.

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
