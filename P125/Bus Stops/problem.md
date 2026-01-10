## Title
Bus Stops

## Slug
bus-stops

## Difficulty
Medium

## Description
Commuters waiting at random points on a road need to walk to established bus stops.

There are $n$ waiting points and $m$ bus stops positioned at specific coordinates along a main road.

The commuter plans to establish a service range. All bus stops will operate with the same walking distance $r$. A bus stop at location $x$ with walking distance $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every waiting point must be covered by at least one bus stop.

Your task is to determine the **minimum non-negative integer walking distance $r$** required to ensure that all $n$ waiting points are within the range of at least one bus stop.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
waiting points are at -2, 2, 4. bus stops are at -3, 0.
With walking distance 4:
- bus stop at -3 covers [-7, 1]. Covers waiting point at -2.
- bus stop at 0 covers [-4, 4]. Covers waiting points at -2, 2, 4.
All waiting points covered. Minimum walking distance is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With walking distance 3:
- bus stop at 4 covers [1, 7]. Covers waiting points 1, 5.
- bus stop at 11 covers [8, 14]. Covers waiting points 10, 14.
- bus stop at 15 covers [12, 18]. Covers waiting point 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of waiting points and bus stops.
- The second line contains $n$ integers representing the coordinates of the waiting points. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the bus stops. The coordinates are sorted in non-decreasing order.

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
