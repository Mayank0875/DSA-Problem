## Title

Median Grid Product

## Slug

median-grid-product

## Difficulty

Medium

## Description

Given an integer n, consider the grid of numbers formed by the first n positive integers as both rows and columns. For each cell (i, j) in this grid, the value is i * j. When all these n * n values are sorted in increasing order, find the value at the central position (since the total number of elements is n² which is odd for odd n).

For example, for n=3, the grid values are:
    [1, 2, 3]
    [2, 4, 6]
    [3, 6, 9]

Sorted: [1,2,2,3,3,4,6,6,9]. The median (the 5th element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list of all products is [1,2,2,3,3,4,6,6,9]. The median (5th element) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

The sorted list of all products for n=5 has 25 elements. The median (13th element) is 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return one integer: the median value.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory