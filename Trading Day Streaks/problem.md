## Title

Trading Day Streaks

## Slug

trading-day-streaks

## Difficulty

Medium

## Description

You are analyzing the performance of a virtual stock market. For each trading day, you want to determine its "streak". The streak for a given day is the maximum number of consecutive days immediately preceding it (including the current day) for which the stock price was less than or equal to the price on the current day. You are given the prices for n consecutive days. Your task is to calculate the streak for each day.

## Examples

### 1

#### Input

7
[100, 80, 60, 70, 60, 75, 85]

#### Output

[1, 1, 1, 2, 1, 4, 6]

#### Explanation

Day 1: Price 100. Streak is 1 (only day 1).
Day 2: Price 80. Streak is 1 (only day 2).
Day 3: Price 60. Streak is 1 (only day 3).
Day 4: Price 70. Price on day 3 (60) <= 70. Streak is 2 (days 3, 4).
Day 5: Price 60. Streak is 1 (only day 5).
Day 6: Price 75. Prices on days 5(60), 4(70), 3(60) <= 75. Streak is 4 (days 3, 4, 5, 6).
Day 7: Price 85. Prices on days 6(75), 5(60), 4(70), 3(60), 2(80) <= 85. Streak is 6 (days 2, 3, 4, 5, 6, 7).

### 2

#### Input

5
[10, 20, 30, 40, 50]

#### Output

[1, 2, 3, 4, 5]

#### Explanation

Day 1: Price 10. Streak is 1.
Day 2: Price 20. Streak is 2.
Day 3: Price 30. Streak is 3.
Day 4: Price 40. Streak is 4.
Day 5: Price 50. Streak is 5.
  

## Input Format  

- The first line contains a single integer n, the number of days.
- The second line contains n space-separated integers, representing the stock prices for each day from day 1 to day n.

## Output Format  

- Return n sized array, where the i-th integer is the streak for day i.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ price ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array