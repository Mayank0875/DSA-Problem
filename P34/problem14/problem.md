## Title

Median of Grid Products

## Slug

median-grid-products

## Description

Given an integer n (which is odd), consider an n x n grid where each cell (i, j) contains the value (i+1) * (j+1). When all these n^2 numbers are sorted in increasing order, the median value is the one exactly in the middle.

For example, for n=3, the grid values are:
[1, 2, 3]
[2, 4, 6]
[3, 6, 9]

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

- Return one integer: the median of the sorted grid products.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory