## Title
Festival Parade Route

## Slug
festival-parade-route

## Difficulty
Hard

## Description
A parade moves through a festival. Starting at the Gate (1), it must reach the Main Stage (n). Performance areas are connected by paths.

The parade must start at the Gate (labeled 1) and finish at the Main Stage (labeled n). However, to entertain the crowd in every area, the parade must visit **every single area exactly once** during the journey.

You are given the map of the areas and the directed paths connecting them. Your task is to calculate the total number of distinct valid paths the parade can take to complete the parade. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every area exactly once:
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
- The first line contains two integers n and m: the number of areas and the number of paths.
- The areas are numbered 1, 2, ..., n.
- The next m lines describe the paths. Each line has two integers a and b, indicating a one-way path from area a to area b.

## Output Format
- Return one integer: the number of possible parade paths modulo 10^9+7.

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
