## Title

Find the Top of the Hill

## Slug

find-top-of-hill

## Difficulty

Medium

## Description

You are given an array of `n` elevation points. The points represent a single hill: they strictly increase to the top, and then strictly decrease.
    1. n >= 3
    2. `elev[0] < elev[1] < ... < elev[i-1] < elev[i]`
    3. `elev[i] > elev[i+1] > ... > elev[n-1]`

Find the index of the top of the hill.

## Examples

### 1

#### Input

7
[0, 1, 2, 4, 2, 1, 0]

#### Output

3

#### Explanation

The array is [0, 1, 2, 4, 2, 1, 0]. The peak element is 4 at index 3.

### 2

#### Input

5
[1, 5, 4, 3, 2]

#### Output

1

#### Explanation

The array is [1, 5, 4, 3, 2]. The peak element is 5 at index 1.

## Input Format

- The first line contains a single integer n, the number of elements in the array.
- The second line contains n space-separated integers, representing the elements of the mountain array arr.

## Output Format

- Return a single integer: the index of the peak element.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ arr[i] ≤ 10^9
- The input array is guaranteed to be a mountain array.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory