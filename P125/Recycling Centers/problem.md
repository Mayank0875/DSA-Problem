## Title
Recycling Centers

## Slug
recycling-centers

## Difficulty
Medium

## Description
Dump sites need to be serviced by recycling centers.

There are $n$ dump sites and $m$ centers positioned at specific coordinates along a highway.

The environmentalist plans to establish a service range. All centers will operate with the same haul radius $r$. A center at location $x$ with haul radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every dump site must be covered by at least one center.

Your task is to determine the **minimum non-negative integer haul radius $r$** required to ensure that all $n$ dump sites are within the range of at least one center.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
dump sites are at -2, 2, 4. centers are at -3, 0.
With haul radius 4:
- center at -3 covers [-7, 1]. Covers dump site at -2.
- center at 0 covers [-4, 4]. Covers dump sites at -2, 2, 4.
All dump sites covered. Minimum haul radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With haul radius 3:
- center at 4 covers [1, 7]. Covers dump sites 1, 5.
- center at 11 covers [8, 14]. Covers dump sites 10, 14.
- center at 15 covers [12, 18]. Covers dump site 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of dump sites and centers.
- The second line contains $n$ integers representing the coordinates of the dump sites. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the centers. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal haul radius $r$ required.

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
