## Title
Luxury Handbags

## Slug
luxury-handbags

## Difficulty
Easy

## Description
Fashionistas track the resale value of Birkin bags. You want to buy one and resell it on a luxury marketplace.

You have a list of bag price for $n$ consecutive months. You want to make one perfect move: purchase on one month and consign on a different month in the future. You cannot consign before you purchase.

Your goal is to find the **maximum possible upside** you can earn from this single transaction. If it is impossible to make any upside (i.e., the bag price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
purchase on month 2 (bag price = 1) and consign on month 5 (bag price = 6). The upside is $6 - 1 = 5$.
Note that purchaseing on month 1 (bag price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The bag price never increases, so it is impossible to make a upside. The maximum upside is 0.

## Input Format
- The first line contains a single integer `n`, the number of months.
- The second line contains `n` space-separated integers representing the bag price on each month.

## Output Format
- Return a single integer representing the maximum upside. If no upside can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
