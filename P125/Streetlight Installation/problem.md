## Title
Streetlight Installation

## Slug
streetlight-installation

## Difficulty
Medium

## Description
A city planner is installing lights along a dark street. The goal is to illuminate specific dark spots using lamp posts placed at fixed locations.

There are $n$ dark spots and $m$ lamp posts positioned at specific coordinates along a straight road.

The planner plans to establish a service range. All lamp posts will operate with the same light radius $r$. A lamp post at location $x$ with light radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every dark spot must be covered by at least one lamp post.

Your task is to determine the **minimum non-negative integer light radius $r$** required to ensure that all $n$ dark spots are within the range of at least one lamp post.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
dark spots are at -2, 2, 4. lamp posts are at -3, 0.
With light radius 4:
- lamp post at -3 covers [-7, 1]. Covers dark spot at -2.
- lamp post at 0 covers [-4, 4]. Covers dark spots at -2, 2, 4.
All dark spots covered. Minimum light radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With light radius 3:
- lamp post at 4 covers [1, 7]. Covers dark spots 1, 5.
- lamp post at 11 covers [8, 14]. Covers dark spots 10, 14.
- lamp post at 15 covers [12, 18]. Covers dark spot 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of dark spots and lamp posts.
- The second line contains $n$ integers representing the coordinates of the dark spots. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the lamp posts. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal light radius $r$ required.

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
