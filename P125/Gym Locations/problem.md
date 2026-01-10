## Title
Gym Locations

## Slug
gym-locations

## Difficulty
Medium

## Description
Residential blocks need to be within jogging distance of a fitness center.

There are $n$ blocks and $m$ gyms positioned at specific coordinates along a city line.

The trainer plans to establish a service range. All gyms will operate with the same jogging distance $r$. A gym at location $x$ with jogging distance $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every block must be covered by at least one gym.

Your task is to determine the **minimum non-negative integer jogging distance $r$** required to ensure that all $n$ blocks are within the range of at least one gym.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
blocks are at -2, 2, 4. gyms are at -3, 0.
With jogging distance 4:
- gym at -3 covers [-7, 1]. Covers block at -2.
- gym at 0 covers [-4, 4]. Covers blocks at -2, 2, 4.
All blocks covered. Minimum jogging distance is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With jogging distance 3:
- gym at 4 covers [1, 7]. Covers blocks 1, 5.
- gym at 11 covers [8, 14]. Covers blocks 10, 14.
- gym at 15 covers [12, 18]. Covers block 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of blocks and gyms.
- The second line contains $n$ integers representing the coordinates of the blocks. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the gyms. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal jogging distance $r$ required.

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
