## Title
Marathon Course Design

## Slug
marathon-course-design

## Difficulty
Hard

## Description
A race organizer plans a route through the city. Starting at the Plaza (1), runners must reach the Stadium (n). Landmarks are connected by streets.

The runner must start at the Plaza (labeled 1) and finish at the Stadium (labeled n). However, to pass every major landmark for the scenic view, the runner must visit **every single landmark exactly once** during the journey.

You are given the map of the landmarks and the directed streets connecting them. Your task is to calculate the total number of distinct valid paths the runner can take to complete the race. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every landmark exactly once:
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
- The first line contains two integers n and m: the number of landmarks and the number of streets.
- The landmarks are numbered 1, 2, ..., n.
- The next m lines describe the streets. Each line has two integers a and b, indicating a one-way street from landmark a to landmark b.

## Output Format
- Return one integer: the number of possible race paths modulo 10^9+7.

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
