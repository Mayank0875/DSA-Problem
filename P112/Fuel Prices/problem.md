## Title
Fuel Prices

## Slug
fuel-prices

## Difficulty
Easy

## Description
A logistics company tracks diesel prices. They want to fill their massive storage tank once when cheap and use it (saving money) when prices are high.

You have a list of fuel cost for $n$ consecutive days. You want to make one perfect move: fill up on one day and consume on a different day in the future. You cannot consume before you fill up.

Your goal is to find the **maximum possible savings** you can earn from this single transaction. If it is impossible to make any savings (i.e., the fuel cost only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
fill up on day 2 (fuel cost = 1) and consume on day 5 (fuel cost = 6). The savings is $6 - 1 = 5$.
Note that fill uping on day 1 (fuel cost = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The fuel cost never increases, so it is impossible to make a savings. The maximum savings is 0.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the fuel cost on each day.

## Output Format
- Return a single integer representing the maximum savings. If no savings can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
