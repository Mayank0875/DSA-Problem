## Title
Security Cameras

## Slug
security-cameras

## Difficulty
Medium

## Description
Valuable exhibits in a long hallway need to be visible to security cameras mounted on the ceiling.

There are $n$ exhibits and $m$ cameras positioned at specific coordinates along a hallway.

The security chief plans to establish a service range. All cameras will operate with the same view radius $r$. A camera at location $x$ with view radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every exhibit must be covered by at least one camera.

Your task is to determine the **minimum non-negative integer view radius $r$** required to ensure that all $n$ exhibits are within the range of at least one camera.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
exhibits are at -2, 2, 4. cameras are at -3, 0.
With view radius 4:
- camera at -3 covers [-7, 1]. Covers exhibit at -2.
- camera at 0 covers [-4, 4]. Covers exhibits at -2, 2, 4.
All exhibits covered. Minimum view radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With view radius 3:
- camera at 4 covers [1, 7]. Covers exhibits 1, 5.
- camera at 11 covers [8, 14]. Covers exhibits 10, 14.
- camera at 15 covers [12, 18]. Covers exhibit 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of exhibits and cameras.
- The second line contains $n$ integers representing the coordinates of the exhibits. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the cameras. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal view radius $r$ required.

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
