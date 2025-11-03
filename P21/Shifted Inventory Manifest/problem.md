## Title

Shifted Inventory Manifest

## Slug

shifted-inventory-manifest

## Difficulty

Medium

## Description

A warehouse stores items sorted by a unique part number. A new employee accidentally "cut" the sorted list, moving a block of items from the end to the front. The manifest now shows a rotated sorted array (e.g., [10, 20, 30] becomes [30, 10, 20]). To fix the manifest, you must find the part number that should be first (the minimum value). Find this value in O(log n) time.

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