## Title
Police Patrols

## Slug
police-patrols

## Difficulty
Medium

## Description
Crime hotspots along a patrol route need to be monitored by police cars stationed at intersections.

There are $n$ hotspots and $m$ police cars positioned at specific coordinates along a patrol route.

The sergeant plans to establish a service range. All police cars will operate with the same response range $r$. A police car at location $x$ with response range $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every hotspot must be covered by at least one police car.

Your task is to determine the **minimum non-negative integer response range $r$** required to ensure that all $n$ hotspots are within the range of at least one police car.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
hotspots are at -2, 2, 4. police cars are at -3, 0.
With response range 4:
- police car at -3 covers [-7, 1]. Covers hotspot at -2.
- police car at 0 covers [-4, 4]. Covers hotspots at -2, 2, 4.
All hotspots covered. Minimum response range is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With response range 3:
- police car at 4 covers [1, 7]. Covers hotspots 1, 5.
- police car at 11 covers [8, 14]. Covers hotspots 10, 14.
- police car at 15 covers [12, 18]. Covers hotspot 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of hotspots and police cars.
- The second line contains $n$ integers representing the coordinates of the hotspots. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the police cars. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal response range $r$ required.

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
