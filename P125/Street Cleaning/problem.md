## Title
Street Cleaning

## Slug
street-cleaning

## Difficulty
Medium

## Description
Dirty patches on a road must be reached by cleaning depots.

There are $n$ dirty patches and $m$ depots positioned at specific coordinates along a road.

The cleaner plans to establish a service range. All depots will operate with the same cleaning radius $r$. A depot at location $x$ with cleaning radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every dirty patch must be covered by at least one depot.

Your task is to determine the **minimum non-negative integer cleaning radius $r$** required to ensure that all $n$ dirty patches are within the range of at least one depot.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
dirty patches are at -2, 2, 4. depots are at -3, 0.
With cleaning radius 4:
- depot at -3 covers [-7, 1]. Covers dirty patch at -2.
- depot at 0 covers [-4, 4]. Covers dirty patches at -2, 2, 4.
All dirty patches covered. Minimum cleaning radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With cleaning radius 3:
- depot at 4 covers [1, 7]. Covers dirty patches 1, 5.
- depot at 11 covers [8, 14]. Covers dirty patches 10, 14.
- depot at 15 covers [12, 18]. Covers dirty patch 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of dirty patches and depots.
- The second line contains $n$ integers representing the coordinates of the dirty patches. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the depots. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal cleaning radius $r$ required.

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
