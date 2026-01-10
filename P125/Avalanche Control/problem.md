## Title
Avalanche Control

## Slug
avalanche-control

## Difficulty
Medium

## Description
Snow build-up zones on a mountain pass need to be targeted by control cannons.

There are $n$ zones and $m$ cannons positioned at specific coordinates along a mountain pass.

The safety officer plans to establish a service range. All cannons will operate with the same firing range $r$. A cannon at location $x$ with firing range $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every zone must be covered by at least one cannon.

Your task is to determine the **minimum non-negative integer firing range $r$** required to ensure that all $n$ zones are within the range of at least one cannon.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
zones are at -2, 2, 4. cannons are at -3, 0.
With firing range 4:
- cannon at -3 covers [-7, 1]. Covers zone at -2.
- cannon at 0 covers [-4, 4]. Covers zones at -2, 2, 4.
All zones covered. Minimum firing range is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With firing range 3:
- cannon at 4 covers [1, 7]. Covers zones 1, 5.
- cannon at 11 covers [8, 14]. Covers zones 10, 14.
- cannon at 15 covers [12, 18]. Covers zone 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of zones and cannons.
- The second line contains $n$ integers representing the coordinates of the zones. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the cannons. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal firing range $r$ required.

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
