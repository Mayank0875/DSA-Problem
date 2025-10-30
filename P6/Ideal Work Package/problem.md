## Title

Ideal Work Package

## Slug

ideal-work-package

## Difficulty

Medium

## Description

A project is broken down into N tasks, arranged linearly. Each task `i` is assigned a "point value" `A[i]` (an integer from 0 to 9) representing its contribution.
An "ideal work package" is a contiguous set of tasks, from L to R, where the total point value of the tasks (`A[L] + ... + A[R]`) is exactly equal to the number of tasks in the package (R - L + 1).
Count the total number of ideal work packages.

Note: The array is 1-based indexed, i.e., the first element is A₁.

## Examples

### 1

#### Input

5
[1, 1, 0, 1, 1]

#### Output

6

#### Explanation

There are 6 ideal work packages: A[1 .. 1], A[2 .. 2], A[1 .. 2], A[4 .. 4], A[5 .. 5], A[4 .. 5]

### 2

#### Input

3
[1, 2, 0]

#### Output

3

#### Explanation

There are 3 ideal work packages: A[1 .. 1], A[2 .. 3], A[1 .. 3]

## Input Format

- The first line contains an integer N, the size of the array. 
- The second line contains N space-separated integers, representing the elements of the array (0 to 9).

## Output Format

- Return a single integer, the number of ideal work packages.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hash map