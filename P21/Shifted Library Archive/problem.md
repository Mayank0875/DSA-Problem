## Title

Shifted Library Archive

## Slug

shifted-library-archive

## Difficulty

Medium

## Description

A set of ancient scrolls, numbered sequentially by year, are stored in an archive. A section of the archive was moved from the end to the beginning, creating a "rotated" sorted list of scroll IDs (e.g., [1, 2, 3, 4, 5] became [4, 5, 1, 2, 3]). Given this list of unique IDs, you must find the ID of the oldest scroll (the minimum value). You must write an algorithm with O(log n) runtime complexity.

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