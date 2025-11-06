## Title

Median of Sorted Matrix

## Slug

median-sorted-matrix

## Difficulty

Medium

## Description

Given a positive odd integer n, consider the n x n multiplication table. Each cell (i, j) (with 1 <= i, j <= n) contains the value i * j. Find the median element when all the n^2 numbers are sorted in non-decreasing order.

For example, when n=3, the matrix is:
    [[1, 2, 3], [2, 4, 6], [3, 6, 9]]

The sorted list is [1,2,2,3,3,4,6,6,9]. The median (the fifth element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list is [1,2,2,3,3,4,6,6,9]. The median (the fifth element) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

For n=5, the sorted list has 25 elements. The median (the 13th element) is 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return one integer: the median of the multiplication table.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory