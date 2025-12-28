## Title
Magic The Gathering

## Slug
magic-the-gathering

## Difficulty
Easy

## Description
A player tracks the price of the 'Black Lotus' card. They want to buy one copy and sell it when collectors are desperate.

You have a list of card price for $n$ consecutive months. You want to make one perfect move: purchase on one month and trade on a different month in the future. You cannot trade before you purchase.

Your goal is to find the **maximum possible value gain** you can earn from this single transaction. If it is impossible to make any value gain (i.e., the card price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
purchase on month 2 (card price = 1) and trade on month 5 (card price = 6). The value gain is $6 - 1 = 5$.
Note that purchaseing on month 1 (card price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The card price never increases, so it is impossible to make a value gain. The maximum value gain is 0.

## Input Format
- The first line contains a single integer `n`, the number of months.
- The second line contains `n` space-separated integers representing the card price on each month.

## Output Format
- Return a single integer representing the maximum value gain. If no value gain can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
