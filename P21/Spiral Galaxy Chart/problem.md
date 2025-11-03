## Title

Spiral Galaxy Chart

## Slug

spiral-galaxy-chart

## Difficulty

Medium

## Description

A spiral galaxy chart lists star systems by their distance from the core, sorted in increasing order. The chart is circular and has been rotated. You are given a list of these unique distances as they appear on the rotated chart (e.g., [10, 20, 30, 40] might be [30, 40, 10, 20]). You need to find the star system closest to the core, which has the minimum distance. Find this minimum value in O(log n) time.

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