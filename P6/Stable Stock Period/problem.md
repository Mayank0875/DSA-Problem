## Title

Stable Stock Period

## Slug

stable-stock-period

## Difficulty

Medium

## Description

You are analyzing stock market data for N consecutive days. For each day `i`, you have a "profit factor" `A[i]`, which is an integer from 0 to 9.
A "stable period" is a contiguous range of days, from day L to day R, where the sum of the profit factors (`A[L] + ... + A[R]`) is exactly equal to the number of days in that period (R - L + 1).
Your goal is to determine how many such stable periods exist in the N-day data.

Note: The array is 1-based indexed, i.e., the first element is A₁.

## Examples

### 1

#### Input

5
[1, 1, 0, 1, 1]

#### Output

6

#### Explanation

There are 6 stable periods: A[1 .. 1], A[2 .. 2], A[1 .. 2], A[4 .. 4], A[5 .. 5], A[4 .. 5]

### 2

#### Input

3
[1, 2, 0]

#### Output

3

#### Explanation

There are 3 stable periods: A[1 .. 1], A[2 .. 3], A[1 .. 3]

## Input Format

- The first line contains an integer N, the size of the array. 
- The second line contains N space-separated integers, representing the elements of the array (0 to 9).

## Output Format

- Return a single integer, the number of stable periods.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hash map