## Title

Matrix Median

## Slug

matrix-median

## Description

Given an integer n, consider the n x n multiplication table. However, instead of numbers, each cell (i, j) (with 1-indexing) contains the value i * j. Now, if we list all the n*n numbers in the table in non-decreasing order, find the median element.

Since n is odd, the median is the element at position (n²+1)/2.

For example, when n = 3, the table is:
Row1: 1, 2, 3
Row2: 2, 4, 6
Row3: 3, 6, 9

The sorted list is [1,2,2,3,3,4,6,6,9]. The median (5th element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list of the 3x3 multiplication table is [1,2,2,3,3,4,6,6,9]. The middle (5th) element is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

The sorted list of the 5x5 multiplication table has 25 elements. The median is the 13th element, which is 8.

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