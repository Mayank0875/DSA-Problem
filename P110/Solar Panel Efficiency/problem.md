## Title
Solar Panel Efficiency

## Slug
solar-panel-efficiency

## Difficulty
Easy

## Description
An engineer tracks power output. A 'Sunrise Curve' is a sequence of minutes where power output strictly increases.

The Engineer is analyzing a sequence of minutes represented by an array of integers `nums`, where `nums[i]` represents the wattage at index `i`.

The Engineer wants to find the maximum total wattage obtained during a single "**Sunrise Curve**". A "Sunrise Curve" is defined as a contiguous subarray of minutes where the wattage of each minute is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of wattages possible from one such Sunrise Curve. The Sunrise Curve must include at least one minute.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Engineer identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Sunrise Curve starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of minutes.
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
