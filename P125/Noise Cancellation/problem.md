## Title
Noise Cancellation

## Slug
noise-cancellation

## Difficulty
Medium

## Description
Loud machinery needs to be dampened by active noise cancellers placed along a factory wall.

There are $n$ machines and $m$ cancellers positioned at specific coordinates along a factory wall.

The engineer plans to establish a service range. All cancellers will operate with the same silence radius $r$. A canceller at location $x$ with silence radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every machine must be covered by at least one canceller.

Your task is to determine the **minimum non-negative integer silence radius $r$** required to ensure that all $n$ machines are within the range of at least one canceller.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
machines are at -2, 2, 4. cancellers are at -3, 0.
With silence radius 4:
- canceller at -3 covers [-7, 1]. Covers machine at -2.
- canceller at 0 covers [-4, 4]. Covers machines at -2, 2, 4.
All machines covered. Minimum silence radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With silence radius 3:
- canceller at 4 covers [1, 7]. Covers machines 1, 5.
- canceller at 11 covers [8, 14]. Covers machines 10, 14.
- canceller at 15 covers [12, 18]. Covers machine 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of machines and cancellers.
- The second line contains $n$ integers representing the coordinates of the machines. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the cancellers. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal silence radius $r$ required.

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
