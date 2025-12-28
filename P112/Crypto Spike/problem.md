## Title
Crypto Spike

## Slug
crypto-spike

## Difficulty
Easy

## Description
You are monitoring a new cryptocurrency called 'MoonCoin'. You want to buy exactly one coin and sell it later to maximize your returns.

You have a list of coin price for $n$ consecutive minutes. You want to make one perfect move: buy on one minute and sell on a different minute in the future. You cannot sell before you buy.

Your goal is to find the **maximum possible profit** you can earn from this single transaction. If it is impossible to make any profit (i.e., the coin price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
buy on minute 2 (coin price = 1) and sell on minute 5 (coin price = 6). The profit is $6 - 1 = 5$.
Note that buying on minute 1 (coin price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The coin price never increases, so it is impossible to make a profit. The maximum profit is 0.

## Input Format
- The first line contains a single integer `n`, the number of minutes.
- The second line contains `n` space-separated integers representing the coin price on each minute.

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
