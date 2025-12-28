## Title
Lego Set

## Slug
lego-set

## Difficulty
Easy

## Description
A collector tracks the price of the Millennium Falcon set. They want to buy it before it retires and sell it later.

You have a list of set price for $n$ consecutive months. You want to make one perfect move: store on one month and flip on a different month in the future. You cannot flip before you store.

Your goal is to find the **maximum possible profit** you can earn from this single transaction. If it is impossible to make any profit (i.e., the set price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
store on month 2 (set price = 1) and flip on month 5 (set price = 6). The profit is $6 - 1 = 5$.
Note that storeing on month 1 (set price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The set price never increases, so it is impossible to make a profit. The maximum profit is 0.

## Input Format
- The first line contains a single integer `n`, the number of months.
- The second line contains `n` space-separated integers representing the set price on each month.

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
