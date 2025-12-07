## Title
Taxi Driver Challenge

## Slug
taxi-driver-challenge

## Difficulty
Hard

## Description
A driver participates in a challenge. Starting at the Garage (1), they must reach the Depot (n). City districts are connected by one-way streets.

The driver must start at the Garage (labeled 1) and finish at the Depot (labeled n). However, to pick up a passenger in every district, the driver must visit **every single district exactly once** during the journey.

You are given the map of the districts and the directed streets connecting them. Your task is to calculate the total number of distinct valid paths the driver can take to complete the challenge. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every district exactly once:
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
- The first line contains two integers n and m: the number of districts and the number of streets.
- The districts are numbered 1, 2, ..., n.
- The next m lines describe the streets. Each line has two integers a and b, indicating a one-way street from district a to district b.

## Output Format
- Return one integer: the number of possible challenge paths modulo 10^9+7.

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
