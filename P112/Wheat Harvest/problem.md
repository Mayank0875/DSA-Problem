## Title
Wheat Harvest

## Slug
wheat-harvest

## Difficulty
Easy

## Description
A miller tracks wheat prices. They want to buy grain futures and sell flour when the market peaks.

You have a list of bushel price for $n$ consecutive months. You want to make one perfect move: contract on one month and supply on a different month in the future. You cannot supply before you contract.

Your goal is to find the **maximum possible net income** you can earn from this single transaction. If it is impossible to make any net income (i.e., the bushel price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
contract on month 2 (bushel price = 1) and supply on month 5 (bushel price = 6). The net income is $6 - 1 = 5$.
Note that contracting on month 1 (bushel price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The bushel price never increases, so it is impossible to make a net income. The maximum net income is 0.

## Input Format
- The first line contains a single integer `n`, the number of months.
- The second line contains `n` space-separated integers representing the bushel price on each month.

## Output Format
- Return a single integer representing the maximum net income. If no net income can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
