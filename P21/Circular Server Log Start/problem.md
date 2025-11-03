## Title

Circular Server Log Start

## Slug

circular-server-log-start

## Difficulty

Medium

## Description

A server cluster's logs are sorted by timestamp. The log system uses a circular buffer. When the buffer fills, it "rolls over," placing the newest log after the oldest. This creates a rotated sorted array of timestamps (e.g., [50, 60, 10, 20, 30]). To find the full time range, you must locate the single oldest timestamp (the minimum value) in the buffer. Find this minimum value in O(log n) time.

## Examples

### 1

#### Input

7
[4, 5, 6, 7, 0, 1, 2]

#### Output

0

#### Explanation

The smallest value in this rotated sequence is 0.

### 2

#### Input

6
[4, 5, 6, 7, 1, 2]

#### Output

1

#### Explanation

The smallest value in this rotated sequence is 1.

## Input Format

- The first line contains an integer n, the number of items.
- The second line contains n space-separated integers representing the item numbers after rotation. All numbers are unique.

## Output Format

- Return a single integer representing the minimum item number found.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ gem_number ≤ 10^9
- The array is guaranteed to be a rotation of a sorted array.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array