## Title
Public Toilets

## Slug
public-toilets

## Difficulty
Medium

## Description
Tourists at attractions along a promenade need access to restrooms.

There are $n$ attractions and $m$ restrooms positioned at specific coordinates along a promenade.

The city council plans to establish a service range. All restrooms will operate with the same convenience radius $r$. A restroom at location $x$ with convenience radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every attraction must be covered by at least one restroom.

Your task is to determine the **minimum non-negative integer convenience radius $r$** required to ensure that all $n$ attractions are within the range of at least one restroom.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
attractions are at -2, 2, 4. restrooms are at -3, 0.
With convenience radius 4:
- restroom at -3 covers [-7, 1]. Covers attraction at -2.
- restroom at 0 covers [-4, 4]. Covers attractions at -2, 2, 4.
All attractions covered. Minimum convenience radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With convenience radius 3:
- restroom at 4 covers [1, 7]. Covers attractions 1, 5.
- restroom at 11 covers [8, 14]. Covers attractions 10, 14.
- restroom at 15 covers [12, 18]. Covers attraction 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of attractions and restrooms.
- The second line contains $n$ integers representing the coordinates of the attractions. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the restrooms. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal convenience radius $r$ required.

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
