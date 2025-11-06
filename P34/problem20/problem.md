## Title

Median of Sorted Matrix

## Slug

sorted-matrix-median

## Description

Given an n x n multiplication table (with n odd), find the median value when all the elements are sorted in increasing order.

For example, for n=3, the multiplication table is:
[[1, 2, 3], [2, 4, 6], [3, 6, 9]]
The sorted list is [1,2,2,3,3,4,6,6,9], so the median is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list is [1,2,2,3,3,4,6,6,9]. The median (the 5th element in a 1-indexed list of 9) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

The sorted list includes numbers from 1 to 25, but with many duplicates. The 13th element (the median) is 8.

## Input Format

- A single integer n.

## Output Format

- The median value.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory