## Title
Fuel Efficiency

## Slug
fuel-efficiency

## Difficulty
Easy

## Description
A driver tests eco-mode. An 'Efficiency Glide' is a sequence of miles where MPG strictly increases.

The Driver is analyzing a sequence of miles represented by an array of integers `nums`, where `nums[i]` represents the MPG at index `i`.

The Driver wants to find the maximum total MPG obtained during a single "**Efficiency Glide**". A "Efficiency Glide" is defined as a contiguous subarray of miles where the MPG of each mile is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of MPGs possible from one such Efficiency Glide. The Efficiency Glide must include at least one mile.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Driver identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Efficiency Glide starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of miles.
- The second line contains `n` space-separated integers, representing the MPGs.

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
