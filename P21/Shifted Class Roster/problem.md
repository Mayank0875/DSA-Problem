## Title

Shifted Class Roster

## Slug

shifted-class-roster

## Difficulty

Medium

## Description

A class roster is sorted by unique student ID. The teacher printed the list but accidentally started from a student in the middle, "rotating" the list (e.t., [10, 11, 12, 13] becomes [12, 13, 10, 11]). To find the student with the lowest ID number, you are given this rotated array. Find the minimum ID in O(log n) time.

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