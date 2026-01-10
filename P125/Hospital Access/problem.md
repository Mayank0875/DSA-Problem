## Title
Hospital Access

## Slug
hospital-access

## Difficulty
Medium

## Description
Remote clinics along a valley road need to be within helicopter range of major hospitals.

There are $n$ clinics and $m$ hospitals positioned at specific coordinates along a valley road.

The health minister plans to establish a service range. All hospitals will operate with the same flight radius $r$. A hospital at location $x$ with flight radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every clinic must be covered by at least one hospital.

Your task is to determine the **minimum non-negative integer flight radius $r$** required to ensure that all $n$ clinics are within the range of at least one hospital.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
clinics are at -2, 2, 4. hospitals are at -3, 0.
With flight radius 4:
- hospital at -3 covers [-7, 1]. Covers clinic at -2.
- hospital at 0 covers [-4, 4]. Covers clinics at -2, 2, 4.
All clinics covered. Minimum flight radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With flight radius 3:
- hospital at 4 covers [1, 7]. Covers clinics 1, 5.
- hospital at 11 covers [8, 14]. Covers clinics 10, 14.
- hospital at 15 covers [12, 18]. Covers clinic 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of clinics and hospitals.
- The second line contains $n$ integers representing the coordinates of the clinics. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the hospitals. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal flight radius $r$ required.

## Constraints
- 1 ≤ n, m ≤ 10^5
- -10^9 ≤ coordinates ≤ 10^9
- The input arrays are sorted in non-decreasing order.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, two-pointers, array, math
