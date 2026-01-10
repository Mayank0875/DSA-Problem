## Title
Parade Viewing

## Slug
parade-viewing

## Difficulty
Medium

## Description
Crowds along a parade route need to see floats passing by certain markers.

There are $n$ crowd groups and $m$ markers positioned at specific coordinates along a parade route.

The spectator plans to establish a service range. All markers will operate with the same viewing distance $r$. A marker at location $x$ with viewing distance $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every crowd group must be covered by at least one marker.

Your task is to determine the **minimum non-negative integer viewing distance $r$** required to ensure that all $n$ crowd groups are within the range of at least one marker.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
crowd groups are at -2, 2, 4. markers are at -3, 0.
With viewing distance 4:
- marker at -3 covers [-7, 1]. Covers crowd group at -2.
- marker at 0 covers [-4, 4]. Covers crowd groups at -2, 2, 4.
All crowd groups covered. Minimum viewing distance is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With viewing distance 3:
- marker at 4 covers [1, 7]. Covers crowd groups 1, 5.
- marker at 11 covers [8, 14]. Covers crowd groups 10, 14.
- marker at 15 covers [12, 18]. Covers crowd group 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of crowd groups and markers.
- The second line contains $n$ integers representing the coordinates of the crowd groups. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the markers. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal viewing distance $r$ required.

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
