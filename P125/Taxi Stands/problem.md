## Title
Taxi Stands

## Slug
taxi-stands

## Difficulty
Medium

## Description
Hotels on a strip need to be served by nearby taxi stands.

There are $n$ hotels and $m$ taxi stands positioned at specific coordinates along a hotel strip.

The planner plans to establish a service range. All taxi stands will operate with the same service radius $r$. A taxi stand at location $x$ with service radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every hotel must be covered by at least one taxi stand.

Your task is to determine the **minimum non-negative integer service radius $r$** required to ensure that all $n$ hotels are within the range of at least one taxi stand.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
hotels are at -2, 2, 4. taxi stands are at -3, 0.
With service radius 4:
- taxi stand at -3 covers [-7, 1]. Covers hotel at -2.
- taxi stand at 0 covers [-4, 4]. Covers hotels at -2, 2, 4.
All hotels covered. Minimum service radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With service radius 3:
- taxi stand at 4 covers [1, 7]. Covers hotels 1, 5.
- taxi stand at 11 covers [8, 14]. Covers hotels 10, 14.
- taxi stand at 15 covers [12, 18]. Covers hotel 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of hotels and taxi stands.
- The second line contains $n$ integers representing the coordinates of the hotels. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the taxi stands. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal service radius $r$ required.

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
