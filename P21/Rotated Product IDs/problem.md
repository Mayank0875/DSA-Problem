## Title

Rotated Product IDs

## Slug

rotated-product-ids

## Difficulty

Medium

## Description

A list of product IDs in a database is sorted. A programming error caused the list to be "rotated," so it now starts from an unknown ID (e.g., [100, 101, 102] became [102, 100, 101]). To re-sort the database, you first need to find the starting point of the original list, which is the product with the minimum ID. Find this minimum ID in O(log n) time.

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