## Title
Crypto Pump

## Slug
crypto-pump

## Difficulty
Easy

## Description
A bot tracks a cryptocurrency. A 'Pump' is a sequence of hourly ticks where the price strictly increases.

The Bot is analyzing a sequence of price ticks represented by an array of integers `nums`, where `nums[i]` represents the value at index `i`.

The Bot wants to find the maximum total value obtained during a single "**Pump**". A "Pump" is defined as a contiguous subarray of price ticks where the value of each tick is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of values possible from one such Pump. The Pump must include at least one tick.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Bot identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Pump starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of price ticks.
- The second line contains `n` space-separated integers, representing the values.

## Output Format
- Return a single integer representing the maximum sum of any strictly increasing contiguous subarray.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ nums[i] ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sliding-window, easy
