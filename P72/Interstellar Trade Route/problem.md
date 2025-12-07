## Title
Interstellar Trade Route

## Slug
interstellar-trade-route

## Difficulty
Hard

## Description
A merchant ship needs to visit every major trading post in a star sector to maximize profits before returning to the base. There are n trading posts connected by one-way hyperlanes.

The ship must start at the Entry Post (labeled 1) and finish at the Exit Post (labeled n). However, to collect specialized goods from each market, the ship must visit **every single trading post exactly once** during the journey.

You are given the map of the trading posts and the directed hyperlanes connecting them. Your task is to calculate the total number of distinct valid paths the ship can take to complete the trade route. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every trading post exactly once:
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
- The first line contains two integers n and m: the number of trading posts and the number of hyperlanes.
- The trading posts are numbered 1, 2, ..., n.
- The next m lines describe the hyperlanes. Each line has two integers a and b, indicating a one-way hyperlane from trading post a to trading post b.

## Output Format
- Return one integer: the number of possible trade route paths modulo 10^9+7.

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
