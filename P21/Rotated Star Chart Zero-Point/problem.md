## Title

Rotated Star Chart Zero-Point

## Slug

rotated-star-chart-zero-point

## Difficulty

Medium

## Description

A deep-space observatory charts stars by a unique ID, sorted in ascending order. The chart is on a circular display that has been spun. The data now appears as a rotated sorted array (e.g., [101, 102, 103] might be [103, 101, 102]). To recalibrate the display, you must find the "zero-point" of the original list, which is the star with the minimum ID. Find this minimum value in O(log n) time.

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