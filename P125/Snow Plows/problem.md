## Title
Snow Plows

## Slug
snow-plows

## Difficulty
Medium

## Description
Snowed-in driveways along a street need to be cleared by plows stationed at intersections.

There are $n$ driveways and $m$ plows positioned at specific coordinates along a street.

The driver plans to establish a service range. All plows will operate with the same operation range $r$. A plow at location $x$ with operation range $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every driveway must be covered by at least one plow.

Your task is to determine the **minimum non-negative integer operation range $r$** required to ensure that all $n$ driveways are within the range of at least one plow.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
driveways are at -2, 2, 4. plows are at -3, 0.
With operation range 4:
- plow at -3 covers [-7, 1]. Covers driveway at -2.
- plow at 0 covers [-4, 4]. Covers driveways at -2, 2, 4.
All driveways covered. Minimum operation range is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With operation range 3:
- plow at 4 covers [1, 7]. Covers driveways 1, 5.
- plow at 11 covers [8, 14]. Covers driveways 10, 14.
- plow at 15 covers [12, 18]. Covers driveway 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of driveways and plows.
- The second line contains $n$ integers representing the coordinates of the driveways. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the plows. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal operation range $r$ required.

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
