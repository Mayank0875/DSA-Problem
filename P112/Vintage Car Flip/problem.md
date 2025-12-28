## Title
Vintage Car Flip

## Slug
vintage-car-flip

## Difficulty
Easy

## Description
You are tracking the auction value of a classic '67 Mustang. You plan to buy it once and sell it later when the market peaks.

You have a list of market value for $n$ consecutive months. You want to make one perfect move: purchase on one month and auction on a different month in the future. You cannot auction before you purchase.

Your goal is to find the **maximum possible return** you can earn from this single transaction. If it is impossible to make any return (i.e., the market value only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
purchase on month 2 (market value = 1) and auction on month 5 (market value = 6). The return is $6 - 1 = 5$.
Note that purchaseing on month 1 (market value = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The market value never increases, so it is impossible to make a return. The maximum return is 0.

## Input Format
- The first line contains a single integer `n`, the number of months.
- The second line contains `n` space-separated integers representing the market value on each month.

## Output Format
- Return a single integer representing the maximum return. If no return can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
