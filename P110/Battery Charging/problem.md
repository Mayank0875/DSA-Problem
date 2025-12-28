## Title
Battery Charging

## Slug
battery-charging

## Difficulty
Easy

## Description
A fast charger pushes power. A 'Ramp Up' is the initial phase where the charging wattage strictly increases every second.

The Technician is analyzing a sequence of seconds represented by an array of integers `nums`, where `nums[i]` represents the wattage at index `i`.

The Technician wants to find the maximum total wattage obtained during a single "**Ramp Up**". A "Ramp Up" is defined as a contiguous subarray of seconds where the wattage of each second is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of wattages possible from one such Ramp Up. The Ramp Up must include at least one second.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Technician identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Ramp Up starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of seconds.
- The second line contains `n` space-separated integers, representing the wattages.

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
