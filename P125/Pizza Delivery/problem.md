## Title
Pizza Delivery

## Slug
pizza-delivery

## Difficulty
Medium

## Description
A pizza chain wants to guarantee delivery to all apartment complexes along a route using their branch locations.

There are $n$ apartments and $m$ branches positioned at specific coordinates along a delivery route.

The franchise owner plans to establish a service range. All branches will operate with the same delivery radius $r$. A branch at location $x$ with delivery radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every apartment must be covered by at least one branch.

Your task is to determine the **minimum non-negative integer delivery radius $r$** required to ensure that all $n$ apartments are within the range of at least one branch.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
apartments are at -2, 2, 4. branches are at -3, 0.
With delivery radius 4:
- branch at -3 covers [-7, 1]. Covers apartment at -2.
- branch at 0 covers [-4, 4]. Covers apartments at -2, 2, 4.
All apartments covered. Minimum delivery radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With delivery radius 3:
- branch at 4 covers [1, 7]. Covers apartments 1, 5.
- branch at 11 covers [8, 14]. Covers apartments 10, 14.
- branch at 15 covers [12, 18]. Covers apartment 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of apartments and branches.
- The second line contains $n$ integers representing the coordinates of the apartments. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the branches. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal delivery radius $r$ required.

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
