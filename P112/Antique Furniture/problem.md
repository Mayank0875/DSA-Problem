## Title
Antique Furniture

## Slug
antique-furniture

## Difficulty
Easy

## Description
An antiquarian tracks the value of Victorian chairs. They want to buy a set and sell it when the style comes back into fashion.

You have a list of market price for $n$ consecutive years. You want to make one perfect move: restore on one year and retail on a different year in the future. You cannot retail before you restore.

Your goal is to find the **maximum possible profit** you can earn from this single transaction. If it is impossible to make any profit (i.e., the market price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
restore on year 2 (market price = 1) and retail on year 5 (market price = 6). The profit is $6 - 1 = 5$.
Note that restoreing on year 1 (market price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The market price never increases, so it is impossible to make a profit. The maximum profit is 0.

## Input Format
- The first line contains a single integer `n`, the number of years.
- The second line contains `n` space-separated integers representing the market price on each year.

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
