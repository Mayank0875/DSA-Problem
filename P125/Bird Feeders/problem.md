## Title
Bird Feeders

## Slug
bird-feeders

## Difficulty
Medium

## Description
Nesting sites in a park need to be close to bird feeders.

There are $n$ nests and $m$ feeders positioned at specific coordinates along a park trail.

The ornithologist plans to establish a service range. All feeders will operate with the same foraging radius $r$. A feeder at location $x$ with foraging radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every nest must be covered by at least one feeder.

Your task is to determine the **minimum non-negative integer foraging radius $r$** required to ensure that all $n$ nests are within the range of at least one feeder.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
nests are at -2, 2, 4. feeders are at -3, 0.
With foraging radius 4:
- feeder at -3 covers [-7, 1]. Covers nest at -2.
- feeder at 0 covers [-4, 4]. Covers nests at -2, 2, 4.
All nests covered. Minimum foraging radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With foraging radius 3:
- feeder at 4 covers [1, 7]. Covers nests 1, 5.
- feeder at 11 covers [8, 14]. Covers nests 10, 14.
- feeder at 15 covers [12, 18]. Covers nest 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of nests and feeders.
- The second line contains $n$ integers representing the coordinates of the nests. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the feeders. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal foraging radius $r$ required.

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
