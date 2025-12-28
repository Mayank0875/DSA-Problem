## Title
Lumber Futures

## Slug
lumber-futures

## Difficulty
Easy

## Description
A contractor watches lumber prices. They want to buy wood for a project and sell the surplus later when prices rise.

You have a list of wood price for $n$ consecutive weeks. You want to make one perfect move: order on one week and resell on a different week in the future. You cannot resell before you order.

Your goal is to find the **maximum possible profit** you can earn from this single transaction. If it is impossible to make any profit (i.e., the wood price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
order on week 2 (wood price = 1) and resell on week 5 (wood price = 6). The profit is $6 - 1 = 5$.
Note that ordering on week 1 (wood price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The wood price never increases, so it is impossible to make a profit. The maximum profit is 0.

## Input Format
- The first line contains a single integer `n`, the number of weeks.
- The second line contains `n` space-separated integers representing the wood price on each week.

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
