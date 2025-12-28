## Title
Fishing Haul

## Slug
fishing-haul

## Difficulty
Easy

## Description
A fisherman catches fish in a sequence. A 'Lucky Streak' occurs when each consecutive fish caught weighs strictly more than the previous one.

The Fisherman is analyzing a sequence of fish represented by an array of integers `nums`, where `nums[i]` represents the weight at index `i`.

The Fisherman wants to find the maximum total weight obtained during a single "**Lucky Streak**". A "Lucky Streak" is defined as a contiguous subarray of fish where the weight of each fish is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of weights possible from one such Lucky Streak. The Lucky Streak must include at least one fish.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Fisherman identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Lucky Streak starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of fish.
- The second line contains `n` space-separated integers, representing the weights.

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
