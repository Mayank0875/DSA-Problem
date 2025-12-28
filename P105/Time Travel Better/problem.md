## Title
Time Travel Better

## Slug
time-travel-better

## Difficulty
Medium

## Description
You have a sports almanac from the future, but the timeline is unstable, causing odds to fluctuate.

You have an array `prices` where `prices[i]` represents the market price of a bet slip on the $i$-th day.

To maximize your winnings, you can perform multiple transactions. A transaction consists of buying one bet slip and selling it on a different day. You must observe the following rules:
1. You can hold **at most one** bet slip at a time.
2. You can buy and sell on the same day (e.g., sell your current bet slip to realize a profit, then immediately buy a new one at the same price).
3. You can perform as many transactions as you like.

Your goal is to calculate the **maximum profit** you can achieve over the given period.

## Examples

### 1

#### Input
6 
7 1 5 3 6 4

#### Output
7

#### Explanation
* Buy on day 2 (price = 1) and sell on day 3 (price = 5), profit = $5 - 1 = 4$.
* Buy on day 4 (price = 3) and sell on day 5 (price = 6), profit = $6 - 3 = 3$.
* Total profit is $4 + 3 = 7$.

### 2

#### Input
5 
1 2 3 4 5

#### Output
4

#### Explanation
* Buy on day 1 (price = 1) and sell on day 5 (price = 5), profit = $5 - 1 = 4$.
* Alternatively, buying and selling every day yields $(2-1) + (3-2) + (4-3) + (5-4) = 4$.

## Input Format
- The first line contains an integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the `prices` array.

## Output Format
- Return a single integer representing the maximum profit.

## Constraints
- 1 ≤ n ≤ 10^4
- 0 ≤ prices[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy
