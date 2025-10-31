## Title

Shortest Rainfall Period

## Slug

shortest-rainfall-period

## Difficulty

Easy

## Description

You are given an array `nums` of positive hourly rainfall amounts (in mm) and a `target` total rainfall. Find the length of the shortest contiguous time period (subarray) where the total rainfall is greater than or equal to `target`. If this amount is never reached, return 0.

## Examples

### 1

#### Input

6 7
[2, 1, 5, 2, 3, 2]

#### Output

2

#### Explanation

The subarray [5, 2] has the minimal length of 2 and its sum is 7, which is equal to the target.

### 2

#### Input

6 8
[2, 1, 5, 2, 3, 2]

#### Output

3

#### Explanation

The subarray [5, 2, 3] has the minimal length of 3 and its sum is 10, which is greater than the target.

## Input Format

- The first line contains two integers n and target, where n is the number of elements in the array.
- The second line contains n space-separated positive integers representing the elements of the array.

## Output Format

- Return a single integer — length of the shortest contiguous subarray

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ target ≤ 10^9
- 0 ≤ arr[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, sliding-window, two-pointers