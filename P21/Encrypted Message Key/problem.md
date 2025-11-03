## Title

Encrypted Message Key

## Slug

encrypted-message-key

## Difficulty

Medium

## Description

An encryption key is a list of unique numbers, originally sorted. The key was "rotated" by a spy as an extra layer of security (e.g., [1, 2, 3, 4, 5] became [3, 4, 5, 1, 2]). To decrypt a message, you must first find the "pivot," which is the smallest number in the sequence. Given the rotated array, find this minimum value in O(log n) time.

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