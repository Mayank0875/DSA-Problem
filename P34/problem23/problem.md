## Title

Grid Product Median

## Slug

grid-product-median

## Difficulty

Medium

## Description

Given an odd integer n, consider an n x n multiplication table where the element at row i and column j is i * j (for i, j from 1 to n). The entries of this table are sorted into a single list in increasing order. Your task is to find the median element of this sorted list.

For example, for n = 3, the multiplication table is:
    [[1, 2, 3], [2, 4, 6], [3, 6, 9]]

The sorted list is [1,2,2,3,3,4,6,6,9], which has 9 elements. The median (the 5th element) is 3.

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

The sorted list has 25 elements. The median (13th element) is 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return the median value.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory