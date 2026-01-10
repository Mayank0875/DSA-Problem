## Title
Stock Market Trading

## Slug
stock-market-trading

## Difficulty
Easy

## Description
An exchange tracks open buy orders.

The order book records the open time and close time of every order in two integer arrays, `startTime` and `endTime`. The $i$-th order is placed at `startTime[i]` and is filled at `endTime[i]`, inclusive.

The trader wants to know how many orders were active during a specific market fluctuation `[queryStart, queryEnd]`. A order is considered active if their lifespan overlaps with the market fluctuation at any point (even for a single moment).

Your task is to return the total number of orders who were active during the given market fluctuation.

## Examples

### 1

#### Input
3
1 2 3
3 2 7
2 4

#### Output
3

#### Explanation
The market fluctuation is `[2, 4]`.
- Order 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Order 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Order 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 orders were active.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The order was active at time `[4, 4]`. The market fluctuation is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of orders.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of orders active during the market fluctuation.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ startTime[i] ≤ endTime[i] ≤ 10^9
- 1 ≤ queryStart ≤ queryEnd ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, interval, linear-scan

## Company
amazon
