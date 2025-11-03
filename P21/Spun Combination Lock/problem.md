## Title

Spun Combination Lock

## Slug

spun-combination-lock

## Difficulty

Medium

## Description

A combination lock has numbers on its dial, sorted in increasing order. The dial has been spun, so the sequence of numbers you see is a rotated sorted array (e.g., [1, 2, 3, 4] becomes [3, 4, 1, 2]). To reset the lock, you need to find the "true zero," which is the smallest number on the dial. Given the array of unique numbers, find this minimum value in O(log n) time.

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