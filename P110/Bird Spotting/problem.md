## Title
Bird Spotting

## Slug
bird-spotting

## Difficulty
Easy

## Description
A birder counts birds seen per day. A 'Migration Wave' is a streak of days where the daily count strictly increases.

The Birder is analyzing a sequence of days represented by an array of integers `nums`, where `nums[i]` represents the bird count at index `i`.

The Birder wants to find the maximum total bird count obtained during a single "**Migration Wave**". A "Migration Wave" is defined as a contiguous subarray of days where the bird count of each day is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of bird counts possible from one such Migration Wave. The Migration Wave must include at least one day.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Birder identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Migration Wave starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers, representing the bird counts.

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
