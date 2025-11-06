## Title

Median of Grid Products

## Slug

median-grid-products

## Difficulty

Medium

## Description

Given an odd integer n, consider an n x n multiplication table where the element at (i, j) is i * j (with i and j starting from 1). Extract all the numbers from this table and sort them in increasing order. Find the median value.

For example, for n = 3, the table is:
    [[1, 2, 3], 
     [2, 4, 6], 
     [3, 6, 9]]
The sorted list is [1,2,2,3,3,4,6,6,9], and the median (the 5th element) is 3.

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

For n=5, the sorted list of all products is [1,2,2,3,3,4,4,4,5,5,6,6,6,7,8,8,8,9,10,10,12,12,15,16,20,25]. The median (13th element) is 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return one integer: the median of the sorted list of products.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory<｜begin▁of▁sentence｜>