## Title
Bee Pollination

## Slug
bee-pollination

## Difficulty
Medium

## Description
Flower patches along a meadow path need pollination from beehives.

There are $n$ flower patches and $m$ hives positioned at specific coordinates along a meadow path.

The beekeeper plans to establish a service range. All hives will operate with the same flight range $r$. A hive at location $x$ with flight range $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every flower patch must be covered by at least one hive.

Your task is to determine the **minimum non-negative integer flight range $r$** required to ensure that all $n$ flower patches are within the range of at least one hive.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
flower patches are at -2, 2, 4. hives are at -3, 0.
With flight range 4:
- hive at -3 covers [-7, 1]. Covers flower patch at -2.
- hive at 0 covers [-4, 4]. Covers flower patches at -2, 2, 4.
All flower patches covered. Minimum flight range is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With flight range 3:
- hive at 4 covers [1, 7]. Covers flower patches 1, 5.
- hive at 11 covers [8, 14]. Covers flower patches 10, 14.
- hive at 15 covers [12, 18]. Covers flower patch 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of flower patches and hives.
- The second line contains $n$ integers representing the coordinates of the flower patches. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the hives. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal flight range $r$ required.

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
