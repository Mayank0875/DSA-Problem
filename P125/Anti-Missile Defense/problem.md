## Title
Anti-Missile Defense

## Slug
anti-missile-defense

## Difficulty
Medium

## Description
Cities along a border need protection from defense batteries.

There are $n$ cities and $m$ batteries positioned at specific coordinates along a border.

The general plans to establish a service range. All batteries will operate with the same interception radius $r$. A battery at location $x$ with interception radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every city must be covered by at least one battery.

Your task is to determine the **minimum non-negative integer interception radius $r$** required to ensure that all $n$ cities are within the range of at least one battery.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
cities are at -2, 2, 4. batteries are at -3, 0.
With interception radius 4:
- battery at -3 covers [-7, 1]. Covers city at -2.
- battery at 0 covers [-4, 4]. Covers cities at -2, 2, 4.
All cities covered. Minimum interception radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With interception radius 3:
- battery at 4 covers [1, 7]. Covers cities 1, 5.
- battery at 11 covers [8, 14]. Covers cities 10, 14.
- battery at 15 covers [12, 18]. Covers city 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of cities and batteries.
- The second line contains $n$ integers representing the coordinates of the cities. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the batteries. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal interception radius $r$ required.

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
