## Title
Forest Fire Watch

## Slug
forest-fire-watch

## Difficulty
Medium

## Description
Dry zones in a forest line need to be visible from watchtowers.

There are $n$ dry zones and $m$ towers positioned at specific coordinates along a forest ridge.

The ranger plans to establish a service range. All towers will operate with the same vision range $r$. A tower at location $x$ with vision range $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every dry zone must be covered by at least one tower.

Your task is to determine the **minimum non-negative integer vision range $r$** required to ensure that all $n$ dry zones are within the range of at least one tower.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
dry zones are at -2, 2, 4. towers are at -3, 0.
With vision range 4:
- tower at -3 covers [-7, 1]. Covers dry zone at -2.
- tower at 0 covers [-4, 4]. Covers dry zones at -2, 2, 4.
All dry zones covered. Minimum vision range is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With vision range 3:
- tower at 4 covers [1, 7]. Covers dry zones 1, 5.
- tower at 11 covers [8, 14]. Covers dry zones 10, 14.
- tower at 15 covers [12, 18]. Covers dry zone 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of dry zones and towers.
- The second line contains $n$ integers representing the coordinates of the dry zones. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the towers. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal vision range $r$ required.

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
