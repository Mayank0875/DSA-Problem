## Title
Fish Market

## Slug
fish-market

## Difficulty
Easy

## Description
A sushi chef watches the price of Bluefin Tuna at the morning auction. They buy a fish and sell cuts later.

You have a list of price per kg for $n$ consecutive days. You want to make one perfect move: bid on one day and serve on a different day in the future. You cannot serve before you bid.

Your goal is to find the **maximum possible profit** you can earn from this single transaction. If it is impossible to make any profit (i.e., the price per kg only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
bid on day 2 (price per kg = 1) and serve on day 5 (price per kg = 6). The profit is $6 - 1 = 5$.
Note that biding on day 1 (price per kg = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The price per kg never increases, so it is impossible to make a profit. The maximum profit is 0.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the price per kg on each day.

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
