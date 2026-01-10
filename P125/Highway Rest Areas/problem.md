## Title
Highway Rest Areas

## Slug
highway-rest-areas

## Difficulty
Medium

## Description
Tired drivers pull over at markers. They need to be close to official rest areas.

There are $n$ stopped cars and $m$ rest areas positioned at specific coordinates along a highway.

The transport dept plans to establish a service range. All rest areas will operate with the same walking distance $r$. A rest area at location $x$ with walking distance $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every stopped car must be covered by at least one rest area.

Your task is to determine the **minimum non-negative integer walking distance $r$** required to ensure that all $n$ stopped cars are within the range of at least one rest area.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
stopped cars are at -2, 2, 4. rest areas are at -3, 0.
With walking distance 4:
- rest area at -3 covers [-7, 1]. Covers stopped car at -2.
- rest area at 0 covers [-4, 4]. Covers stopped cars at -2, 2, 4.
All stopped cars covered. Minimum walking distance is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With walking distance 3:
- rest area at 4 covers [1, 7]. Covers stopped cars 1, 5.
- rest area at 11 covers [8, 14]. Covers stopped cars 10, 14.
- rest area at 15 covers [12, 18]. Covers stopped car 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of stopped cars and rest areas.
- The second line contains $n$ integers representing the coordinates of the stopped cars. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the rest areas. The coordinates are sorted in non-decreasing order.

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
