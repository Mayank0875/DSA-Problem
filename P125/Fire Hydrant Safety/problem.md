## Title
Fire Hydrant Safety

## Slug
fire-hydrant-safety

## Difficulty
Medium

## Description
A fire department ensures safety along a residential avenue. Houses must be reachable by hydrants located at intervals.

There are $n$ houses and $m$ hydrants positioned at specific coordinates along a avenue.

The chief plans to establish a service range. All hydrants will operate with the same hose length $r$. A hydrant at location $x$ with hose length $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every house must be covered by at least one hydrant.

Your task is to determine the **minimum non-negative integer hose length $r$** required to ensure that all $n$ houses are within the range of at least one hydrant.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
houses are at -2, 2, 4. hydrants are at -3, 0.
With hose length 4:
- hydrant at -3 covers [-7, 1]. Covers house at -2.
- hydrant at 0 covers [-4, 4]. Covers houses at -2, 2, 4.
All houses covered. Minimum hose length is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With hose length 3:
- hydrant at 4 covers [1, 7]. Covers houses 1, 5.
- hydrant at 11 covers [8, 14]. Covers houses 10, 14.
- hydrant at 15 covers [12, 18]. Covers house 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of houses and hydrants.
- The second line contains $n$ integers representing the coordinates of the houses. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the hydrants. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal hose length $r$ required.

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
