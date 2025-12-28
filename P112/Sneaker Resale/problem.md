## Title
Sneaker Resale

## Slug
sneaker-resale

## Difficulty
Easy

## Description
A hypebeast monitors the resale price of limited edition sneakers. They want to buy a pair and resell it for the highest markup.

You have a list of resale price for $n$ consecutive days. You want to make one perfect move: cop on one day and flip on a different day in the future. You cannot flip before you cop.

Your goal is to find the **maximum possible profit** you can earn from this single transaction. If it is impossible to make any profit (i.e., the resale price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
cop on day 2 (resale price = 1) and flip on day 5 (resale price = 6). The profit is $6 - 1 = 5$.
Note that coping on day 1 (resale price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The resale price never increases, so it is impossible to make a profit. The maximum profit is 0.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the resale price on each day.

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
