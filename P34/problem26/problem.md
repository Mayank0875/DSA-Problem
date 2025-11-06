## Title

Matrix Median

## Slug

matrix-median

## Description

In an n * n multiplication table, each element at (i, j) is i * j (with both i and j starting from 1). When all these n² numbers are sorted in non-decreasing order, find the value at the middle position. Assume n is odd.

For example, for n=3, the multiplication table is:
[[1,2,3],[2,4,6],[3,6,9]]
The sorted list is [1,2,2,3,3,4,6,6,9]. The median is the 5th element (since there are 9 elements), which is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list has 9 elements: [1,2,2,3,3,4,6,6,9]. The median is the 5th element, which is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

The sorted list has 25 elements. The median is the 13th element (since (25+1)/2=13), which is 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return one integer: the median of the sorted multiplication table.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory