## Title
Radio Beacons

## Slug
radio-beacons

## Difficulty
Medium

## Description
Ships navigating a narrow strait need to be within range of coastal radio beacons.

There are $n$ ships and $m$ beacons positioned at specific coordinates along a strait.

The coast guard plans to establish a service range. All beacons will operate with the same broadcast range $r$. A beacon at location $x$ with broadcast range $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every ship must be covered by at least one beacon.

Your task is to determine the **minimum non-negative integer broadcast range $r$** required to ensure that all $n$ ships are within the range of at least one beacon.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
ships are at -2, 2, 4. beacons are at -3, 0.
With broadcast range 4:
- beacon at -3 covers [-7, 1]. Covers ship at -2.
- beacon at 0 covers [-4, 4]. Covers ships at -2, 2, 4.
All ships covered. Minimum broadcast range is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With broadcast range 3:
- beacon at 4 covers [1, 7]. Covers ships 1, 5.
- beacon at 11 covers [8, 14]. Covers ships 10, 14.
- beacon at 15 covers [12, 18]. Covers ship 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of ships and beacons.
- The second line contains $n$ integers representing the coordinates of the ships. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the beacons. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal broadcast range $r$ required.

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
