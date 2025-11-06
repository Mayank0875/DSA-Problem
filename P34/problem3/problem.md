## Title

Median of Ordered Products

## Slug

median-ordered-products

## Description

Given an integer n, which is odd, the n x n multiplication table contains n² elements. When sorted in increasing order, the median is the element at position (n² + 1) / 2. Calculate that value.

For example, for n=3, the multiplication table is:
    [[1, 2, 3], [2, 4, 6], [3, 6, 9]]
When sorted, the sequence is [1, 2, 2, 3, 3, 4, 6, 6, 9]. The median is the 5th element (since (9+1)/2 = 5), which is 3.

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

The sorted list of 25 numbers has the 13th element (since (25+1)/2 = 13) as 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return one integer: the median of the sorted products.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory