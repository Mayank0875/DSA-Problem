## Title

The Intergalactic Crystal Trader

## Slug

the-intergalactic-crystal-trader

## Difficulty

Easy

## Description

In the bustling markets of the Andromeda galaxy, traders deal in rare Starlight Crystals. The value of these crystals fluctuates wildly from day to day based on cosmic radiation levels.

You are a novice trader looking to make a quick fortune. You have access to a predictive chart that shows the price of a Starlight Crystal for a sequence of upcoming days. To maximize your credits, you must choose exactly **one day** to buy a single crystal and a **different day in the future** to sell that crystal.

You are given an integer array `prices` where `prices[i]` is the cost of a Starlight Crystal on the $i^{th}$ day.

Your task is to determine the maximum profit you can achieve from this single transaction. If no profit can be made (i.e., prices only go down or stay the same), your profit is `0`.

## Examples

### 1

#### Input

6
[7, 1, 5, 3, 6, 4]

#### Output

5

#### Explanation

Buy on day 2 (price = 1) and sell on day 5 (price = 6), profit = $6 - 1 = 5$.
Note that buying on day 2 and selling on day 1 is not allowed because you must buy before you sell.
    
### 2

#### Input

5 
[7, 6, 4, 3, 1]

#### Output

0

#### Explanation

In this case, no transaction is done because the price drops every day, so the maximum profit is 0.
  

## Input Format  

- The first line contains an integer $n$, the number of days.
- The second line contains $n$ space-separated integers representing the `prices`.

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