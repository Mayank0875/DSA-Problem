## Title

Hill Climb Race Apex

## Slug

hill-climb-race-apex

## Difficulty

Medium

## Description

You are given the altitude readings for a hill climb race. The `n` readings form a "mountain array": the altitude strictly increases to the summit, and then strictly decreases.
    1. n >= 3
    2. `alt[0] < alt[1] < ... < alt[i-1] < alt[i]`
    3. `alt[i] > alt[i+1] > ... > alt[n-1]`

Find the index of the summit (the point of maximum altitude).

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