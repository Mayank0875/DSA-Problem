## Title

Best Weather Period

## Slug

best-weather-period

## Difficulty

Medium

## Description

You are planning an outdoor festival and have a weather forecast for N days. A '1' represents a sunny day, and a '0' represents a rainy day. The festival is "successful" if any contiguous stretch of days has no more than `k` rainy days. What is the length of the longest possible successful festival period?

## Examples

### 1

#### Input

10 2
[1, 1, 0, 1, 0, 1, 1, 1, 0, 1]

#### Output

8

#### Explanation

The given stream is [1, 1, 0, 1, 0, 1, 1, 1, 0, 1] and k=2. The longest subarray with at most two 0s is `[1, 1, 0, 1, 0, 1, 1, 1], which starts at index 1. This subarray contains exactly two 0s and has a length of 8.


### 2

#### Input

8 0
[0, 0, 1, 1, 1, 0, 0, 1]

#### Output

3

#### Explanation

Here, k = 0, which means we are looking for the longest contiguous subarray containing only 1s. 
The longest such subarray is [1, 1, 1], which has a length of 3.


## Input Format

- The first line contains two space-separated integers, n and k, representing the total number of packets and the maximum allowed errors in a stable segment.
- The second line contains n space-separated integers, representing the binary data stream.

## Output Format

- Return a single integer — the length of the longest stable transmission segment.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ k ≤ N
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, two pointers