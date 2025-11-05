## Title

Peak Signal Strength

## Slug

peak-signal-strength

## Difficulty

Medium

## Description

You are an engineer analyzing a signal. The signal's strength readings are stored in a "peak array". A peak array `arr` of size `n` has these properties:
    1. n >= 3
    2. The signal strength increases to a maximum and then decreases.
    3. `arr[0] < arr[1] < ... < arr[i-1] < arr[i]`
    4. `arr[i] > arr[i+1] > ... > arr[n-1]`

Your task is to find the index of the peak signal strength.

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