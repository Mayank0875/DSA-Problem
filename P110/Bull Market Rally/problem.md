## Title
Bull Market Rally

## Slug
bull-market-rally

## Difficulty
Easy

## Description
A stock trader is reviewing historical price charts. They want to identify the most profitable 'Bull Run'—a period where stock prices closed higher every single day consecutively.

The Trader is analyzing a sequence of daily prices represented by an array of integers `nums`, where `nums[i]` represents the price value at index `i`.

The Trader wants to find the maximum total price value obtained during a single "**Bull Run**". A "Bull Run" is defined as a contiguous subarray of daily prices where the price value of each day is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of price values possible from one such Bull Run. The Bull Run must include at least one day.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Trader identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Bull Run starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of daily prices.
- The second line contains `n` space-separated integers, representing the price values.

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
