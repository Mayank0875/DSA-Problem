## Title
Diamond Trade

## Slug
diamond-trade

## Difficulty
Easy

## Description
A gemologist tracks the price of raw diamonds. They want to buy a stone and sell it after cutting and polishing.

You have a list of carat price for $n$ consecutive weeks. You want to make one perfect move: procure on one week and deal on a different week in the future. You cannot deal before you procure.

Your goal is to find the **maximum possible profit** you can earn from this single transaction. If it is impossible to make any profit (i.e., the carat price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
procure on week 2 (carat price = 1) and deal on week 5 (carat price = 6). The profit is $6 - 1 = 5$.
Note that procureing on week 1 (carat price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The carat price never increases, so it is impossible to make a profit. The maximum profit is 0.

## Input Format
- The first line contains a single integer `n`, the number of weeks.
- The second line contains `n` space-separated integers representing the carat price on each week.

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
