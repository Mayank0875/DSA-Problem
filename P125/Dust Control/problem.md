## Title
Dust Control

## Slug
dust-control

## Difficulty
Medium

## Description
Dusty patches on a mining road need to be sprayed by water trucks stationed at intervals.

There are $n$ dusty patches and $m$ trucks positioned at specific coordinates along a mining road.

The foreman plans to establish a service range. All trucks will operate with the same spray reach $r$. A truck at location $x$ with spray reach $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every dusty patch must be covered by at least one truck.

Your task is to determine the **minimum non-negative integer spray reach $r$** required to ensure that all $n$ dusty patches are within the range of at least one truck.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
dusty patches are at -2, 2, 4. trucks are at -3, 0.
With spray reach 4:
- truck at -3 covers [-7, 1]. Covers dusty patch at -2.
- truck at 0 covers [-4, 4]. Covers dusty patches at -2, 2, 4.
All dusty patches covered. Minimum spray reach is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With spray reach 3:
- truck at 4 covers [1, 7]. Covers dusty patches 1, 5.
- truck at 11 covers [8, 14]. Covers dusty patches 10, 14.
- truck at 15 covers [12, 18]. Covers dusty patch 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of dusty patches and trucks.
- The second line contains $n$ integers representing the coordinates of the dusty patches. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the trucks. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal spray reach $r$ required.

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
