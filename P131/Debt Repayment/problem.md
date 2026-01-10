## Title
Debt Repayment

## Slug
debt-repayment

## Difficulty
Medium

## Description
You are paying off a loan. The bank has a strange rule: you can only make a payment equal to a non-zero digit of your current outstanding balance.

You start with a **balance** of `n`. The goal is to reduce this balance to exactly 0.

In one **payment**, you can look at the digits of the current balance, choose one **non-zero digit**, and subtract it from the current balance.

For example, if the balance is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of payments required to reduce the balance to 0.

## Examples

### 1

#### Input
27

#### Output
5

#### Explanation
1. 27 - 7 = 20
2. 20 - 2 = 18
3. 18 - 8 = 10
4. 10 - 1 = 9
5. 9 - 9 = 0
Total payments: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The balance is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of payments.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
