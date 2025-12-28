## Title
Heat Wave Intensity

## Slug
heat-wave-intensity

## Difficulty
Easy

## Description
A meteorologist tracks daily temperatures. A 'Heat Spike' is defined as a sequence of days where the temperature strictly rises each day.

The Scientist is analyzing a sequence of temperatures represented by an array of integers `nums`, where `nums[i]` represents the degree at index `i`.

The Scientist wants to find the maximum total degree obtained during a single "**Heat Spike**". A "Heat Spike" is defined as a contiguous subarray of temperatures where the degree of each day is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of degrees possible from one such Heat Spike. The Heat Spike must include at least one day.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Scientist identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Heat Spike starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of temperatures.
- The second line contains `n` space-separated integers, representing the degrees.

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
