## Title

Median of Grid Products

## Slug

median-grid-products

## Description

Given an odd integer n, consider the n x n multiplication table where the cell (i, j) contains the product i * j (with rows and columns indexed from 1 to n). When all the n^2 numbers in this table are sorted in increasing order, find the element at the middle position (i.e., the median).

For example, for n = 3:
- The multiplication table is:
  1 2 3
  2 4 6
  3 6 9
- The sorted list is [1,2,2,3,3,4,6,6,9], which has 9 elements. The median (the 5th element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list of all products is [1,2,2,3,3,4,6,6,9]. The median (the 5th element) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

For n=5, the sorted list of products has 25 elements. The median (the 13th element) is 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return one integer: the median of the sorted list of products.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory<｜begin▁of▁sentence｜>