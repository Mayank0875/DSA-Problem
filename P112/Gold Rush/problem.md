## Title
Gold Rush

## Slug
gold-rush

## Difficulty
Easy

## Description
A prospector tracks the daily price of gold nuggets. To fund his retirement, he wants to buy gold on a low day and sell it on a high day.

You have a list of gold price for $n$ consecutive days. You want to make one perfect move: buy on one day and sell on a different day in the future. You cannot sell before you buy.

Your goal is to find the **maximum possible earnings** you can earn from this single transaction. If it is impossible to make any earnings (i.e., the gold price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
buy on day 2 (gold price = 1) and sell on day 5 (gold price = 6). The earnings is $6 - 1 = 5$.
Note that buying on day 1 (gold price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The gold price never increases, so it is impossible to make a earnings. The maximum earnings is 0.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the gold price on each day.

## Output Format
- Return a single integer representing the maximum earnings. If no earnings can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
