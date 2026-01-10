## Title
Park Access

## Slug
park-access

## Difficulty
Medium

## Description
Apartment complexes need to be near a green park.

There are $n$ complexes and $m$ parks positioned at specific coordinates along a boulevard.

The urban planner plans to establish a service range. All parks will operate with the same proximity $r$. A park at location $x$ with proximity $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every complex must be covered by at least one park.

Your task is to determine the **minimum non-negative integer proximity $r$** required to ensure that all $n$ complexes are within the range of at least one park.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
complexes are at -2, 2, 4. parks are at -3, 0.
With proximity 4:
- park at -3 covers [-7, 1]. Covers complex at -2.
- park at 0 covers [-4, 4]. Covers complexes at -2, 2, 4.
All complexes covered. Minimum proximity is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With proximity 3:
- park at 4 covers [1, 7]. Covers complexes 1, 5.
- park at 11 covers [8, 14]. Covers complexes 10, 14.
- park at 15 covers [12, 18]. Covers complex 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of complexes and parks.
- The second line contains $n$ integers representing the coordinates of the complexes. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the parks. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal proximity $r$ required.

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
