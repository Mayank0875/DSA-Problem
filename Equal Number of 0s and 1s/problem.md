## Title

Equal Number of 0s and 1s

## Slug

equal-number-01

## Difficulty

Easy

## Description

Given a binary array nums, return the length of the longest contiguous subarray that contains an equal number of 0s and 1s.


## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

[0, 1] is the longest contiguous subarray with an equal number of 0s and 1s.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] and [1, 0] are the longest contiguous subarrays with an equal number of 0s and 1s.


## Input Format

- The first line contains a single integer N, the number of elements in the data stream.
- The second line contains N space-separated integers, where each integer is either 0 or 1.

## Output Format

- Return single integer representing the length of the longest contiguous subarray with an equal number of 0s and 1s.


## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, prefix sum, hashmap