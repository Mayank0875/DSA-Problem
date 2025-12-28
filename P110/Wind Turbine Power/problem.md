## Title
Wind Turbine Power

## Slug
wind-turbine-power

## Difficulty
Easy

## Description
A turbine adjusts to wind. A 'Gust Response' is a period where power generation strictly increases.

The Operator is analyzing a sequence of readings represented by an array of integers `nums`, where `nums[i]` represents the power output at index `i`.

The Operator wants to find the maximum total power output obtained during a single "**Gust Response**". A "Gust Response" is defined as a contiguous subarray of readings where the power output of each reading is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of power outputs possible from one such Gust Response. The Gust Response must include at least one reading.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Operator identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Gust Response starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of readings.
- The second line contains `n` space-separated integers, representing the power outputs.

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
