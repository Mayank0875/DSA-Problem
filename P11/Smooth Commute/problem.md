## Title

Smooth Commute

## Slug

smooth-commute

## Difficulty

Medium

## Description

A traffic camera records N minutes of traffic flow. '1' means traffic is flowing freely, and '0' means it is jammed. A driver is considered to have a "smooth commute" if any continuous segment of their drive has at most `k` minutes of jammed traffic. Find the length of the longest possible smooth commute.

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