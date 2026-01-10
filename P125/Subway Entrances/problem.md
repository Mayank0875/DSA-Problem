## Title
Subway Entrances

## Slug
subway-entrances

## Difficulty
Medium

## Description
Office towers on a grid line need to be close to a subway entrance.

There are $n$ towers and $m$ entrances positioned at specific coordinates along a avenue.

The commuter plans to establish a service range. All entrances will operate with the same walking distance $r$. A entrance at location $x$ with walking distance $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every tower must be covered by at least one entrance.

Your task is to determine the **minimum non-negative integer walking distance $r$** required to ensure that all $n$ towers are within the range of at least one entrance.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
towers are at -2, 2, 4. entrances are at -3, 0.
With walking distance 4:
- entrance at -3 covers [-7, 1]. Covers tower at -2.
- entrance at 0 covers [-4, 4]. Covers towers at -2, 2, 4.
All towers covered. Minimum walking distance is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With walking distance 3:
- entrance at 4 covers [1, 7]. Covers towers 1, 5.
- entrance at 11 covers [8, 14]. Covers towers 10, 14.
- entrance at 15 covers [12, 18]. Covers tower 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of towers and entrances.
- The second line contains $n$ integers representing the coordinates of the towers. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the entrances. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal walking distance $r$ required.

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
