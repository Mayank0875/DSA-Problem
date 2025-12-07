## Title
Concert Tour Logistics

## Slug
concert-tour-logistics

## Difficulty
Hard

## Description
A band plans a tour. Starting at City 1, they must reach the Grand Finale City (n). Cities are connected by flight routes.

The band must start at the City 1 (labeled 1) and finish at the City n (labeled n). However, to perform in every city booked, the band must visit **every single city exactly once** during the journey.

You are given the map of the cities and the directed flights connecting them. Your task is to calculate the total number of distinct valid paths the band can take to complete the tour. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every city exactly once:
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
- The first line contains two integers n and m: the number of cities and the number of flights.
- The cities are numbered 1, 2, ..., n.
- The next m lines describe the flights. Each line has two integers a and b, indicating a one-way flight from city a to city b.

## Output Format
- Return one integer: the number of possible tour paths modulo 10^9+7.

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
