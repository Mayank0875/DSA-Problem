## Title

Balanced Painting

## Slug

balanced-painting

## Difficulty

Medium

## Description

An artist is creating a painting on a long canvas divided into N segments. For each segment `i`, they use a "color intensity" `A[i]` (an integer from 0 to 9).
A "balanced region" is a contiguous sequence of segments, from L to R, where the sum of the color intensities (`A[L] + ... + A[R]`) is exactly equal to the number of segments in that region (R - L + 1).
Find the total number of balanced regions in the painting.

Note: The array is 1-based indexed, i.e., the first element is A₁.

## Examples

### 1

#### Input

5
[1, 1, 0, 1, 1]

#### Output

6

#### Explanation

There are 6 balanced regions: A[1 .. 1], A[2 .. 2], A[1 .. 2], A[4 .. 4], A[5 .. 5], A[4 .. 5]

### 2

#### Input

3
[1, 2, 0]

#### Output

3

#### Explanation

There are 3 balanced regions: A[1 .. 1], A[2 .. 3], A[1 .. 3]

## Input Format

- The first line contains an integer N, the size of the array. 
- The second line contains N space-separated integers, representing the elements of the array (0 to 9).

## Output Format

- Return a single integer, the number of balanced regions.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hash map