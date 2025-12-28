## Title
Retro Console

## Slug
retro-console

## Difficulty
Easy

## Description
A gamer tracks the price of a pristine GameCube. They want to buy it and sell it when nostalgia peaks.

You have a list of console price for $n$ consecutive years. You want to make one perfect move: hunt on one year and eBay on a different year in the future. You cannot eBay before you hunt.

Your goal is to find the **maximum possible profit** you can earn from this single transaction. If it is impossible to make any profit (i.e., the console price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
hunt on year 2 (console price = 1) and eBay on year 5 (console price = 6). The profit is $6 - 1 = 5$.
Note that hunting on year 1 (console price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The console price never increases, so it is impossible to make a profit. The maximum profit is 0.

## Input Format
- The first line contains a single integer `n`, the number of years.
- The second line contains `n` space-separated integers representing the console price on each year.

## Output Format
- Return a single integer representing the maximum profit. If no profit can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
