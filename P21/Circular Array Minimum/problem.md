## Title

Circular Array Minimum

## Slug

circular-array-minimum

## Difficulty

Medium

## Description

You are given an array of unique numbers that was formed by taking a sorted array and "rotating" it. This means a pivot point was chosen, and the elements from that point to the end were moved to the beginning. For example, [0, 1, 2, 4, 5, 6, 7] might become [4, 5, 6, 7, 0, 1, 2]. Your task is to find the smallest element in this rotated array. You must write an algorithm with O(log n) runtime complexity.

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