## Title
Mountain Climber Route

## Slug
mountain-climber-route

## Difficulty
Hard

## Description
A climber ascends a mountain range. Starting at Base Camp (1), they must reach the Summit (n). Camps are connected by climbing routes.

The climber must start at the Base Camp (labeled 1) and finish at the Summit (labeled n). However, to inspect every camp's supplies, the climber must visit **every single camp exactly once** during the journey.

You are given the map of the camps and the directed routes connecting them. Your task is to calculate the total number of distinct valid paths the climber can take to complete the ascent. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every camp exactly once:
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
- The first line contains two integers n and m: the number of camps and the number of routes.
- The camps are numbered 1, 2, ..., n.
- The next m lines describe the routes. Each line has two integers a and b, indicating a one-way route from camp a to camp b.

## Output Format
- Return one integer: the number of possible ascent paths modulo 10^9+7.

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
