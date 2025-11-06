## Title

Median Matrix Multiplication

## Slug

median-matrix-mult

## Description

Given an integer n, which is odd, the matrix of size n x n is defined such that the element at (i, j) is (i+1) * (j+1) for i,j in [0, n-1]. However, the matrix is then sorted into a single list of n*n elements in non-decreasing order. Find the median element of this sorted list.

For example, for n=3:
- The matrix elements are: 
  row0: 1, 2, 3
  row1: 2, 4, 6
  row2: 3, 6, 9
- Sorted list: [1,2,2,3,3,4,6,6,9] 
- Median element is 3.

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
The sorted list of 25 numbers has the 13th element (the median) as 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return the median value (an integer).

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory