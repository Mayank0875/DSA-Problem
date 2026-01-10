## Title
Warehouse Supply

## Slug
warehouse-supply

## Difficulty
Medium

## Description
Retail stores along a logistics corridor must be served by distribution centers.

There are $n$ stores and $m$ centers positioned at specific coordinates along a corridor.

The logistics lead plans to establish a service range. All centers will operate with the same service range $r$. A center at location $x$ with service range $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every store must be covered by at least one center.

Your task is to determine the **minimum non-negative integer service range $r$** required to ensure that all $n$ stores are within the range of at least one center.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
stores are at -2, 2, 4. centers are at -3, 0.
With service range 4:
- center at -3 covers [-7, 1]. Covers store at -2.
- center at 0 covers [-4, 4]. Covers stores at -2, 2, 4.
All stores covered. Minimum service range is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With service range 3:
- center at 4 covers [1, 7]. Covers stores 1, 5.
- center at 11 covers [8, 14]. Covers stores 10, 14.
- center at 15 covers [12, 18]. Covers store 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of stores and centers.
- The second line contains $n$ integers representing the coordinates of the stores. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the centers. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal service range $r$ required.

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
