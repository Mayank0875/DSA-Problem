## Title
Signal Strength

## Slug
signal-strength

## Difficulty
Easy

## Description
A radio operator searches for a signal. A 'Lock-On' event happens when the signal strength strictly increases with each frequency step.

The Operator is analyzing a sequence of steps represented by an array of integers `nums`, where `nums[i]` represents the signal strength at index `i`.

The Operator wants to find the maximum total signal strength obtained during a single "**Lock-On**". A "Lock-On" is defined as a contiguous subarray of steps where the signal strength of each step is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of signal strengths possible from one such Lock-On. The Lock-On must include at least one step.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Operator identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Lock-On starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of steps.
- The second line contains `n` space-separated integers, representing the signal strengths.

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
