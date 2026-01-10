## Title
Lighthouses

## Slug
lighthouses

## Difficulty
Medium

## Description
Dangerous rocks along a coast need to be illuminated by lighthouses.

There are $n$ rocks and $m$ lighthouses positioned at specific coordinates along a coast.

The sailor plans to establish a service range. All lighthouses will operate with the same light range $r$. A lighthouse at location $x$ with light range $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every rock must be covered by at least one lighthouse.

Your task is to determine the **minimum non-negative integer light range $r$** required to ensure that all $n$ rocks are within the range of at least one lighthouse.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
rocks are at -2, 2, 4. lighthouses are at -3, 0.
With light range 4:
- lighthouse at -3 covers [-7, 1]. Covers rock at -2.
- lighthouse at 0 covers [-4, 4]. Covers rocks at -2, 2, 4.
All rocks covered. Minimum light range is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With light range 3:
- lighthouse at 4 covers [1, 7]. Covers rocks 1, 5.
- lighthouse at 11 covers [8, 14]. Covers rocks 10, 14.
- lighthouse at 15 covers [12, 18]. Covers rock 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of rocks and lighthouses.
- The second line contains $n$ integers representing the coordinates of the rocks. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the lighthouses. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal light range $r$ required.

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
