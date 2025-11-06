## Title

Median of Matrix Products

## Slug

median-matrix-products

## Difficulty

Medium

## Description

Given an odd integer n, consider the n * n multiplication table. The table has n rows and n columns, where the element at row i and column j is i * j (for 1-indexed indices). The entire table, when flattened and sorted in increasing order, has a unique median element. Your task is to find that median.

For example, for n = 3, the multiplication table is:
    [[1, 2, 3], [2, 4, 6], [3, 6, 9]]

The sorted list is [1,2,2,3,3,4,6,6,9], and the median (the 5th element in 1-based indexing) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The table has 9 elements. The sorted list is [1,2,2,3,3,4,6,6,9], and the median (5th element) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

The table has 25 elements. The median (13th element) is 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return one integer: the median of the sorted elements from the n * n multiplication table.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory