## Title
Drone Delivery

## Slug
drone-delivery

## Difficulty
Medium

## Description
Customers along a delivery route need to be within range of drone launch bases.

There are $n$ customers and $m$ bases positioned at specific coordinates along a route.

The operator plans to establish a service range. All bases will operate with the same flight radius $r$. A base at location $x$ with flight radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every customer must be covered by at least one base.

Your task is to determine the **minimum non-negative integer flight radius $r$** required to ensure that all $n$ customers are within the range of at least one base.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
customers are at -2, 2, 4. bases are at -3, 0.
With flight radius 4:
- base at -3 covers [-7, 1]. Covers customer at -2.
- base at 0 covers [-4, 4]. Covers customers at -2, 2, 4.
All customers covered. Minimum flight radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With flight radius 3:
- base at 4 covers [1, 7]. Covers customers 1, 5.
- base at 11 covers [8, 14]. Covers customers 10, 14.
- base at 15 covers [12, 18]. Covers customer 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of customers and bases.
- The second line contains $n$ integers representing the coordinates of the customers. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the bases. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal flight radius $r$ required.

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
