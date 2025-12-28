## Title
Call Center Volume

## Slug
call-center-volume

## Difficulty
Easy

## Description
A supervisor tracks active calls. A 'Morning Surge' is a sequence of intervals where call volume strictly increases.

The Supervisor is analyzing a sequence of intervals represented by an array of integers `nums`, where `nums[i]` represents the call count at index `i`.

The Supervisor wants to find the maximum total call count obtained during a single "**Morning Surge**". A "Morning Surge" is defined as a contiguous subarray of intervals where the call count of each interval is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of call counts possible from one such Morning Surge. The Morning Surge must include at least one interval.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Supervisor identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Morning Surge starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of intervals.
- The second line contains `n` space-separated integers, representing the call counts.

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
