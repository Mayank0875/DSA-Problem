## Title
Computer Memory

## Slug
computer-memory

## Difficulty
Easy

## Description
RAM prices fluctuate wildly. A PC builder wants to buy a stock of RAM sticks and sell them when the shortage peaks.

You have a list of RAM price for $n$ consecutive weeks. You want to make one perfect move: stock up on one week and liquidate on a different week in the future. You cannot liquidate before you stock up.

Your goal is to find the **maximum possible revenue** you can earn from this single transaction. If it is impossible to make any revenue (i.e., the RAM price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
stock up on week 2 (RAM price = 1) and liquidate on week 5 (RAM price = 6). The revenue is $6 - 1 = 5$.
Note that stock uping on week 1 (RAM price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The RAM price never increases, so it is impossible to make a revenue. The maximum revenue is 0.

## Input Format
- The first line contains a single integer `n`, the number of weeks.
- The second line contains `n` space-separated integers representing the RAM price on each week.

## Output Format
- Return a single integer representing the maximum revenue. If no revenue can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
