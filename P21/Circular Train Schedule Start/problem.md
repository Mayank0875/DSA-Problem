## Title

Circular Train Schedule Start

## Slug

circular-train-schedule-start

## Difficulty

Medium

## Description

A train schedule lists arrival times (as unique integers) sorted from earliest to latest. The schedule is for a circular route, and the printed list starts at an arbitrary station. This results in a rotated sorted array (e.g., [100, 200, 300, 400] becomes [300, 400, 100, 200]). To find the first train of the day, you must find the minimum time in this list. Find this value in O(log n) time.

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