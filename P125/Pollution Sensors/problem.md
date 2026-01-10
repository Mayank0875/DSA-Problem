## Title
Pollution Sensors

## Slug
pollution-sensors

## Difficulty
Medium

## Description
Factories emitting smoke need to be monitored by air quality sensors.

There are $n$ factories and $m$ sensors positioned at specific coordinates along a industrial zone.

The inspector plans to establish a service range. All sensors will operate with the same detection radius $r$. A sensor at location $x$ with detection radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every factory must be covered by at least one sensor.

Your task is to determine the **minimum non-negative integer detection radius $r$** required to ensure that all $n$ factories are within the range of at least one sensor.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
factories are at -2, 2, 4. sensors are at -3, 0.
With detection radius 4:
- sensor at -3 covers [-7, 1]. Covers factory at -2.
- sensor at 0 covers [-4, 4]. Covers factories at -2, 2, 4.
All factories covered. Minimum detection radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With detection radius 3:
- sensor at 4 covers [1, 7]. Covers factories 1, 5.
- sensor at 11 covers [8, 14]. Covers factories 10, 14.
- sensor at 15 covers [12, 18]. Covers factory 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of factories and sensors.
- The second line contains $n$ integers representing the coordinates of the factories. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the sensors. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal detection radius $r$ required.

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
