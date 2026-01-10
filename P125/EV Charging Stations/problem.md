## Title
EV Charging Stations

## Slug
ev-charging-stations

## Difficulty
Medium

## Description
Electric vehicles are stranded at various mile markers. Tow trucks are stationed at service depots and need to reach them.

There are $n$ stranded cars and $m$ depots positioned at specific coordinates along a interstate.

The dispatcher plans to establish a service range. All depots will operate with the same towing range $r$. A depot at location $x$ with towing range $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every stranded car must be covered by at least one depot.

Your task is to determine the **minimum non-negative integer towing range $r$** required to ensure that all $n$ stranded cars are within the range of at least one depot.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
stranded cars are at -2, 2, 4. depots are at -3, 0.
With towing range 4:
- depot at -3 covers [-7, 1]. Covers stranded car at -2.
- depot at 0 covers [-4, 4]. Covers stranded cars at -2, 2, 4.
All stranded cars covered. Minimum towing range is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With towing range 3:
- depot at 4 covers [1, 7]. Covers stranded cars 1, 5.
- depot at 11 covers [8, 14]. Covers stranded cars 10, 14.
- depot at 15 covers [12, 18]. Covers stranded car 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of stranded cars and depots.
- The second line contains $n$ integers representing the coordinates of the stranded cars. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the depots. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal towing range $r$ required.

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
