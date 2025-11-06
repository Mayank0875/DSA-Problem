## Title

Median of Sorted Matrix

## Slug

median-sorted-matrix

## Description

Given an odd integer n, consider an n x n matrix where each element at (i, j) is i * j (with rows and columns starting at 1). When all elements of this matrix are sorted into a single list in increasing order, find the value at the middle position (since the total number of elements is n², which is odd).

For example, for n = 3, the matrix is:
[[1, 2, 3],
 [2, 4, 6],
 [3, 6, 9]]

The sorted list is [1, 2, 2, 3, 3, 4, 6, 6, 9], so the median (the 5th element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list is [1,2,2,3,3,4,6,6,9]. The median (5th element) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

The sorted list for n=5 has 25 elements. The median (13th element) is 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return one integer: the answer to the task.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory