## Title

Grid Summation Median

## Slug

grid-summation-median

## Difficulty

Medium

## Description

Find the median element when the numbers in an n * n addition table are sorted in increasing order. It is assumed that n is odd.

The n * n addition table is defined such that the element at row i and column j is (i+1) + (j+1), for i, j from 0 to n-1. For example, for n=3, the table is:
    [[2, 3, 4], [3, 4, 5], [4, 5, 6]]

The numbers in increasing order are [2,3,3,4,4,4,5,5,6], so the median is 4.

## Examples

### 1

#### Input

3

#### Output

4

#### Explanation

The numbers in increasing order are [2,3,3,4,4,4,5,5,6], so the median is 4.

### 2

#### Input

5

#### Output

8

#### Explanation

The sorted list of all 25 numbers has 8 as its 13th element (the median).

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

binary-search, math, number-theory<｜begin▁of▁sentence｜>