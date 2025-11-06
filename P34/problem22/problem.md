## Title

Median of Matrix Products

## Slug

median-matrix-products

## Description

Given an odd integer n, consider the n * n multiplication table where the element at row i and column j is i * j (with i, j from 1 to n). 

Find the median of all n^2 elements in this table.

For example, the 3 * 3 multiplication table is:
[[1, 2, 3], [2, 4, 6], [3, 6, 9]]

The elements sorted are [1,2,2,3,3,4,6,6,9]. The median (the middle element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

There are 9 elements. When sorted, the 5th element (the median) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation
The sorted list of the 25 elements has 13 as the median (the 13th element). For n=5, the median value is 8.

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