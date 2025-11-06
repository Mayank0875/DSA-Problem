## Title

Midpoint of Sorted Grid Products

## Slug

sorted-grid-products-midpoint

## Difficulty

Medium

## Description

Given an integer n (which is odd), consider the n x n multiplication table where the element at (i, j) is i * j (for i, j from 1 to n). When all the n * n elements are sorted in non-decreasing order, find the value at the middle position. Since n is odd, n*n is also odd, so there is a single middle element.

For example, for n=3, the multiplication table is:
Row1: [1, 2, 3]
Row2: [2, 4, 6]
Row3: [3, 6, 9]

When sorted, the sequence is [1,2,2,3,3,4,6,6,9]. The middle element (the 5th element, since there are 9 elements) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list is [1,2,2,3,3,4,6,6,9]. The middle (5th) element is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

The sorted list has 25 elements. The 13th element (the middle one) is 8.

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