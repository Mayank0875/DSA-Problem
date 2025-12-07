## Title
Secret Society Initiation

## Slug
secret-society-initiation

## Difficulty
Hard

## Description
An initiate navigates a labyrinth. Starting at the Antechamber (1), they must reach the Inner Sanctum (n). Chambers are connected by hidden passages.

The initiate must start at the Antechamber (labeled 1) and finish at the Inner Sanctum (labeled n). However, to perform a ritual in every room, the initiate must visit **every single chamber exactly once** during the journey.

You are given the map of the chambers and the directed passages connecting them. Your task is to calculate the total number of distinct valid paths the initiate can take to complete the initiation. As the number of paths can be very large, print the answer modulo 1000000007.

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
- The first line contains two integers n and m: the number of chambers and the number of passages.
- The chambers are numbered 1, 2, ..., n.
- The next m lines describe the passages. Each line has two integers a and b, indicating a one-way passage from chamber a to chamber b.

## Output Format
- Return one integer: the number of possible initiation paths modulo 10^9+7.

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
