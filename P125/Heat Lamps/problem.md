## Title
Heat Lamps

## Slug
heat-lamps

## Difficulty
Medium

## Description
Reptiles in a long terrarium need warmth. Heat lamps are placed at fixed sockets.

There are $n$ reptiles and $m$ lamps positioned at specific coordinates along a terrarium.

The zookeeper plans to establish a service range. All lamps will operate with the same heat radius $r$. A lamp at location $x$ with heat radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every reptile must be covered by at least one lamp.

Your task is to determine the **minimum non-negative integer heat radius $r$** required to ensure that all $n$ reptiles are within the range of at least one lamp.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
reptiles are at -2, 2, 4. lamps are at -3, 0.
With heat radius 4:
- lamp at -3 covers [-7, 1]. Covers reptile at -2.
- lamp at 0 covers [-4, 4]. Covers reptiles at -2, 2, 4.
All reptiles covered. Minimum heat radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With heat radius 3:
- lamp at 4 covers [1, 7]. Covers reptiles 1, 5.
- lamp at 11 covers [8, 14]. Covers reptiles 10, 14.
- lamp at 15 covers [12, 18]. Covers reptile 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of reptiles and lamps.
- The second line contains $n$ integers representing the coordinates of the reptiles. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the lamps. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal heat radius $r$ required.

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
