## Title

Consistent Training Block

## Slug

consistent-training-block

## Difficulty

Medium

## Description

An athlete has a training plan spanning N days. On each day `i`, they log an "effort level" `A[i]` (an integer from 0 to 9).
A "consistent block" of training is a contiguous period of days, from L to R, where the total effort level (`A[L] + ... + A[R]`) is exactly equal to the number of days in the block (R - L + 1).
Please determine the total number of consistent blocks in the athlete's N-day plan.

Note: The array is 1-based indexed, i.e., the first element is A₁.

## Examples

### 1

#### Input

5
[1, 1, 0, 1, 1]

#### Output

6

#### Explanation

There are 6 consistent blocks: A[1 .. 1], A[2 .. 2], A[1 .. 2], A[4 .. 4], A[5 .. 5], A[4 .. 5]

### 2

#### Input

3
[1, 2, 0]

#### Output

3

#### Explanation

There are 3 consistent blocks: A[1 .. 1], A[2 .. 3], A[1 .. 3]

## Input Format

- The first line contains an integer N, the size of the array. 
- The second line contains N space-separated integers, representing the elements of the array (0 to 9).

## Output Format

- Return a single integer, the number of consistent blocks.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hash map