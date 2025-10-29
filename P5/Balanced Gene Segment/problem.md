## Title

Stable Transmission Window

## Slug

stable-transmission-window

## Difficulty

Easy

## Description

During data transmission, a sequence of bits (0s and 1s) is sent. Errors can sometimes occur, but certain patterns might indicate stability. We define a "stable window" as a contiguous part of the transmission sequence where the number of 0s equals the number of 1s. Your goal is to analyze a given transmission sequence and find the length of the longest stable window within it.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The window [0, 1] is the longest stable window.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] and [1, 0] are the longest stable windows.

## Input Format

- The first line contains a single integer N, the length of the transmission sequence.
- The second line contains N space-separated integers (bits), either 0 or 1.

## Output Format

- Return a single integer representing the length of the longest contiguous stable window.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, networking, prefix sum, hashmap