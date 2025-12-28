## Title
Video Game Skin

## Slug
video-game-skin

## Difficulty
Easy

## Description
A gamer tracks the marketplace price for a rare knife skin. They want to buy it and sell it when supply runs dry.

You have a list of skin price for $n$ consecutive days. You want to make one perfect move: snipe on one day and list on a different day in the future. You cannot list before you snipe.

Your goal is to find the **maximum possible profit** you can earn from this single transaction. If it is impossible to make any profit (i.e., the skin price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
snipe on day 2 (skin price = 1) and list on day 5 (skin price = 6). The profit is $6 - 1 = 5$.
Note that snipeing on day 1 (skin price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The skin price never increases, so it is impossible to make a profit. The maximum profit is 0.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the skin price on each day.

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
