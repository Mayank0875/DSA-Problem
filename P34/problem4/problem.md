## Title

Matrix Median

## Slug

matrix-median

## Difficulty

Medium

## Description

Given an integer n, consider the n x n multiplication table where the element at row i and column j is i * j (for i, j from 1 to n). Find the median of all the n^2 numbers in this table. Since n is odd, the median is the ((n^2 + 1)/2)-th smallest number.

For example, for n = 3, the multiplication table is:
[[1, 2, 3]
 [2, 4, 6]
 [3, 6, 9]]

The sorted list of all elements is [1,2,2,3,3,4,6,6,9]. There are 9 elements, so the median is the 5th element, which is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list of numbers from the multiplication table is [1,2,2,3,3,4,6,6,9]. The median (5th element) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

For n=5, there are 25 elements. The median is the 13th smallest element, which is 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return one integer: the median value.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory