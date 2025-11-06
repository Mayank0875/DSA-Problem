## Title

Matrix Median

## Slug

matrix-median

## Difficulty

Medium

## Description

Given an n x n multiplication table (where n is odd), determine the median value when all entries are sorted in non-decreasing order. 

For example, for n = 3, the multiplication table is:
    [[1, 2, 3], 
     [2, 4, 6], 
     [3, 6, 9]]

The sorted list becomes [1,2,2,3,3,4,6,6,9]. The median (the fifth element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list of all entries is [1,2,2,3,3,4,6,6,9]. The 5th element (the median) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

For n=5, the sorted list has 25 elements. The 13th element (the median) is 8.

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