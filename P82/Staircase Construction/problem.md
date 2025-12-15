## Title
Staircase Construction

## Slug
staircase-construction

## Difficulty
Easy

## Description
A mason has n stone slabs of different heights. They want to build a staircase where each step is strictly higher.

You have heights of n slabs.
A staircase consists of slabs where each slab is strictly taller than the previous one.

You must build the stairs to find the longest possible staircase. You can skip any number of slabs to form the sequence, but you must maintain the original pile order of the selected slabs. Calculate the maximum number of slabs that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest staircases (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8
The length of these sequences is 4.

### 2

#### Input
5
5 4 3 2 1

#### Output
1

#### Explanation
Since the values are strictly decreasing, we can pick at most 1 slab.

## Input Format
- The first line contains an integer n: the number of slabs.
- The second line contains n integers x_1, x_2 ... x_n: the height of each slab in order.

## Output Format
- Return one integer: the length of the longest valid staircase.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
