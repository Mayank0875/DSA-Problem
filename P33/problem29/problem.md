## Title

Heat Wave Peak

## Slug

heat-wave-peak

## Difficulty

Medium

## Description

You are given the daily high temperatures over `n` days during a heat wave. The temperature strictly increases to a peak, and then strictly decreases.
    1. n >= 3
    2. `temp[0] < temp[1] < ... < temp[i-1] < temp[i]`
    3. `temp[i] > temp[i+1] > ... > temp[n-1]`

Find the index of the hottest day.

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