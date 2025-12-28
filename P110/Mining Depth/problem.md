## Title
Mining Depth

## Slug
mining-depth

## Difficulty
Easy

## Description
A drill records depth progress per hour. A 'Soft Soil Streak' is found when the depth drilled strictly increases each hour.

The Miner is analyzing a sequence of hours represented by an array of integers `nums`, where `nums[i]` represents the depth metered at index `i`.

The Miner wants to find the maximum total depth metered obtained during a single "**Soft Soil Streak**". A "Soft Soil Streak" is defined as a contiguous subarray of hours where the depth metered of each hour is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of depth metereds possible from one such Soft Soil Streak. The Soft Soil Streak must include at least one hour.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Miner identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Soft Soil Streak starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of hours.
- The second line contains `n` space-separated integers, representing the depth metereds.

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
