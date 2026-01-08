## Title
Currency Exchange

## Slug
currency-exchange

## Difficulty
Hard

## Description
A trader moves funds through a chain of banks. Transfers can go to the next bank or skip an intermediary bank.

The trader starts at bank 0 and wishes to reach bank $n$. On each move, The trader can transfer forward either **1 bank** or **2 banks**.

Your task is to calculate the total number of distinct ways to reach exactly bank $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach bank 2:
1. 1 bank + 1 bank
2. 2 banks

### 2

#### Input
3

#### Output
3

#### Explanation
There are three ways:
1. 1 + 1 + 1
2. 1 + 2
3. 2 + 1

## Input Format
- The only input line has an integer $n$ — the target bank.

## Output Format
- Return a single integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math

