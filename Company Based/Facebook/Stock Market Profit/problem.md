## Title

Stock Market Profit

## Slug

stock-market-profit

## Difficulty

Easy

## Description

You are an aspiring investor tracking a single stock. You have a list of its prices for $n$ consecutive days. You want to make one perfect trade: buy on one day and sell on a different day in the future. You cannot sell before you buy. Your goal is to find the maximum possible profit you can earn from this single buy-sell transaction. If it is impossible to make any profit (i.e., the price only goes down), you should return 0.

## Examples

### 1

#### Input

6
[7, 1, 5, 3, 6, 4]

#### Output

5

#### Explanation

Buy on day 2 (price = 1) and sell on day 5 (price = 6). The profit is 6 - 1 = 5.
Note that buying on day 1 (price 7) is not a good choice, as all future prices are lower.
    
### 2

#### Input

5 
[7, 6, 4, 3, 1]

#### Output

0

#### Explanation

The stock price never increases, so it is impossible to make a profit. The maximum profit is 0.
  

## Input Format  

- The first line contains a single integer n, the number of days.
- The second line contains n space-separated integers, prices_i, the price of the stock on day i (where the first day is i=0).

## Output Format  

- Return single integer representing the maximum profit. If no profit can be made, return 0.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ price[i] ≤ 1e4

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, dynamic-programming