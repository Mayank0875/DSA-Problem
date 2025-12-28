## Title
Stock Dividends

## Slug
stock-dividends

## Difficulty
Medium

## Description
Profits are shared. The Major Shareholder takes the bulk, the Minor Shareholder (you) takes the rest, and the Public gets pennies.

There are $3n$ payouts of varying cash available. The distribution follows a strict protocol. In each round, you must select any 3 payouts. The parties then claim them based on the following rules:

1. The **Major** takes the payout with the **maximum** cash from the triplet.
2. You, the **Minor**, take the payout with the **second maximum** cash.
3. The **Public** takes the remaining payout (the one with the minimum cash).

This process repeats until all payouts are distributed. Your goal as the Minor is to maximize the total cash of the payouts you acquire.

Given an array of integers `payouts`, where `payouts[i]` represents the cash of the $i$-th payout, return the maximum total cash you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 payouts. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Major takes `8`, you take `7`, Public takes `2`.
2. Pick the remaining `(1, 2, 4)`. Major takes `4`, you take `2`, Public takes `1`.
Total cash = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Major takes `5`, you take `4`, Public takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of payouts.
- The second line contains $3n$ space-separated integers representing the `payouts` array.

## Output Format
- Return a single integer representing the maximum total cash you can collect.

## Constraints
- 1 ≤ payouts.length ≤ 10^5
- `payouts.length` is divisible by 3.
- 1 ≤ payouts[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
