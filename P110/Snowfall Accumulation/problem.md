## Title
Snowfall Accumulation

## Slug
snowfall-accumulation

## Difficulty
Easy

## Description
A weather station measures snow per hour. A 'Blizzard Intensification' is a period where hourly snowfall strictly increases.

The Meteorologist is analyzing a sequence of hours represented by an array of integers `nums`, where `nums[i]` represents the inch count at index `i`.

The Meteorologist wants to find the maximum total inch count obtained during a single "**Blizzard Intensification**". A "Blizzard Intensification" is defined as a contiguous subarray of hours where the inch count of each hour is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of inch counts possible from one such Blizzard Intensification. The Blizzard Intensification must include at least one hour.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Meteorologist identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Blizzard Intensification starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

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
- The second line contains `n` space-separated integers, representing the inch counts.

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
