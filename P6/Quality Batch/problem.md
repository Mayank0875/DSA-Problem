## Title

Quality Batch

## Slug

quality-batch

## Difficulty

Medium

## Description

A factory's conveyor belt has N items in a row, indexed 1 to N. Each item `i` is given a "quality score" `A[i]` (an integer from 0 to 9).
A "quality batch" is a contiguous group of items, from L to R, where the total quality score (`A[L] + ... + A[R]`) is exactly equal to the number of items in the batch (R - L + 1).
Your job is to count the total number of quality batches on the conveyor belt.

Note: The array is 1-based indexed, i.e., the first element is A₁.

## Examples

### 1

#### Input

5
[1, 1, 0, 1, 1]

#### Output

6

#### Explanation

There are 6 quality batches: A[1 .. 1], A[2 .. 2], A[1 .. 2], A[4 .. 4], A[5 .. 5], A[4 .. 5]

### 2

#### Input

3
[1, 2, 0]

#### Output

3

#### Explanation

There are 3 quality batches: A[1 .. 1], A[2 .. 3], A[1 .. 3]

## Input Format

- The first line contains an integer N, the size of the array. 
- The second line contains N space-separated integers, representing the elements of the array (0 to 9).

## Output Format

- Return a single integer, the number of quality batches.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hash map