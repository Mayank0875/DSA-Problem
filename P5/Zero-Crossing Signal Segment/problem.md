## Title

Zero-Crossing Signal Segment

## Slug

zero-crossing-signal-segment

## Difficulty

Easy

## Description

A digital signal alternates between positive (represented by 1) and negative (represented by 0) polarity levels. An engineer is interested in finding the longest continuous segment of the signal that has perfect balance, meaning it contains an equal number of positive and negative polarity readings. This could indicate a zero-crossing or a specific type of oscillation. Given the signal polarity sequence, find the length of the longest balanced segment.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The segment [0, 1] (Negative, Positive) is the longest balanced segment.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] (Negative, Positive) and [1, 0] (Positive, Negative) are the longest balanced segments.

## Input Format

- The first line contains a single integer N, the length of the signal sequence.
- The second line contains N space-separated integers, representing polarity (0 for negative, 1 for positive).

## Output Format

- Return a single integer representing the length of the longest contiguous balanced segment.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, signal processing, prefix sum, hashmap