## Title

Balanced Garden Row

## Slug

balanced-garden-row

## Difficulty

Medium

## Description

A farmer has planted N plots of land in a single row, indexed 1 to N. Each plot `i` has a "growth yield" value `A[i]` (an integer from 0 to 9).
A "balanced row" is a contiguous subarray of plots, from L to R, where the total growth yield from those plots (`A[L] + ... + A[R]`) is exactly equal to the number of plots in that row (R - L + 1).
You need to calculate the total number of balanced rows in the farmer's field.

Note: The array is 1-based indexed, i.e., the first element is A₁.

## Examples

### 1

#### Input

5
[1, 1, 0, 1, 1]

#### Output

6

#### Explanation

There are 6 balanced rows: A[1 .. 1], A[2 .. 2], A[1 .. 2], A[4 .. 4], A[5 .. 5], A[4 .. 5]

### 2

#### Input

3
[1, 2, 0]

#### Output

3

#### Explanation

There are 3 balanced rows: A[1 .. 1], A[2 .. 3], A[1 .. 3]

## Input Format

- The first line contains an integer N, the size of the array. 
- The second line contains N space-separated integers, representing the elements of the array (0 to 9).

## Output Format

- Return a single integer, the number of balanced rows.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hash map