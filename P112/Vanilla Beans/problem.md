## Title
Vanilla Beans

## Slug
vanilla-beans

## Difficulty
Easy

## Description
A spice trader tracks vanilla prices in Madagascar. They want to buy a harvest and sell it after a cyclone spikes prices.

You have a list of kilo price for $n$ consecutive months. You want to make one perfect move: import on one month and export on a different month in the future. You cannot export before you import.

Your goal is to find the **maximum possible profit** you can earn from this single transaction. If it is impossible to make any profit (i.e., the kilo price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
import on month 2 (kilo price = 1) and export on month 5 (kilo price = 6). The profit is $6 - 1 = 5$.
Note that importing on month 1 (kilo price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The kilo price never increases, so it is impossible to make a profit. The maximum profit is 0.

## Input Format
- The first line contains a single integer `n`, the number of months.
- The second line contains `n` space-separated integers representing the kilo price on each month.

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
