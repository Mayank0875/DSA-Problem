## Title
Archaeological Expedition

## Slug
archaeological-expedition

## Difficulty
Hard

## Description
An explorer navigates ancient ruins. Starting at the Entrance (1), they must reach the Vault (n). The ruins consist of chambers connected by one-way slides or drops.

The explorer must start at the Entrance (labeled 1) and finish at the Vault (labeled n). However, to document every chamber, the explorer must visit **every single chamber exactly once** during the journey.

You are given the map of the chambers and the directed paths connecting them. Your task is to calculate the total number of distinct valid paths the explorer can take to complete the expedition. As the number of paths can be very large, print the answer modulo 1000000007.

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
- The first line contains two integers n and m: the number of chambers and the number of paths.
- The chambers are numbered 1, 2, ..., n.
- The next m lines describe the paths. Each line has two integers a and b, indicating a one-way path from chamber a to chamber b.

## Output Format
- Return one integer: the number of possible expedition paths modulo 10^9+7.

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
