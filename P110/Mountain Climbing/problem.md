## Title
Mountain Climbing

## Slug
mountain-climbing

## Difficulty
Easy

## Description
A climber records elevation gain at checkpoints. A 'Vertical Push' is a series of checkpoints where the elevation gained is strictly higher than the previous check.

The Climber is analyzing a sequence of checkpoints represented by an array of integers `nums`, where `nums[i]` represents the elevation gain at index `i`.

The Climber wants to find the maximum total elevation gain obtained during a single "**Vertical Push**". A "Vertical Push" is defined as a contiguous subarray of checkpoints where the elevation gain of each checkpoint is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of elevation gains possible from one such Vertical Push. The Vertical Push must include at least one checkpoint.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Climber identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Vertical Push starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of checkpoints.
- The second line contains `n` space-separated integers, representing the elevation gains.

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
