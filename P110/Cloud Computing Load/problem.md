## Title
Cloud Computing Load

## Slug
cloud-computing-load

## Difficulty
Easy

## Description
A server admin monitors CPU usage. A 'Load Spike' is a sequence of minutes where CPU usage strictly increases.

The Admin is analyzing a sequence of minutes represented by an array of integers `nums`, where `nums[i]` represents the CPU percentage at index `i`.

The Admin wants to find the maximum total CPU percentage obtained during a single "**Load Spike**". A "Load Spike" is defined as a contiguous subarray of minutes where the CPU percentage of each minute is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of CPU percentages possible from one such Load Spike. The Load Spike must include at least one minute.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Admin identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Load Spike starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

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
- The second line contains `n` space-separated integers, representing the CPU percentages.

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
