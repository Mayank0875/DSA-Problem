## Title
Download Speed

## Slug
download-speed

## Difficulty
Easy

## Description
A user watches a file download. A 'Connection Boost' is a sequence of seconds where the download rate (MB/s) strictly increases.

The User is analyzing a sequence of seconds represented by an array of integers `nums`, where `nums[i]` represents the speed (MB/s) at index `i`.

The User wants to find the maximum total speed (MB/s) obtained during a single "**Connection Boost**". A "Connection Boost" is defined as a contiguous subarray of seconds where the speed (MB/s) of each second is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of speed (MB/s)s possible from one such Connection Boost. The Connection Boost must include at least one second.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The User identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Connection Boost starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

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
- The second line contains `n` space-separated integers, representing the speed (MB/s)s.

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
