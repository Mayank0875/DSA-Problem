## Title

Mountain Range Low Point

## Slug

mountain-range-low-point

## Difficulty

Medium

## Description

A list of mountain peak altitudes was originally sorted. A cartographer's circular map starts from an arbitrary peak, creating a rotated sorted list (e.g., [1000, 2000, 3000] might be [3000, 1000, 2000]). You are given this list of unique altitudes. To find the lowest peak in the range, you must find the minimum value in the array. This must be done in O(log n) time.

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