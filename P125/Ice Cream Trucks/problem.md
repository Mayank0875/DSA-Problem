## Title
Ice Cream Trucks

## Slug
ice-cream-trucks

## Difficulty
Medium

## Description
Playgrounds along a beach need to be served by ice cream trucks parked at lots.

There are $n$ playgrounds and $m$ trucks positioned at specific coordinates along a beach road.

The vendor plans to establish a service range. All trucks will operate with the same serving radius $r$. A truck at location $x$ with serving radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every playground must be covered by at least one truck.

Your task is to determine the **minimum non-negative integer serving radius $r$** required to ensure that all $n$ playgrounds are within the range of at least one truck.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
playgrounds are at -2, 2, 4. trucks are at -3, 0.
With serving radius 4:
- truck at -3 covers [-7, 1]. Covers playground at -2.
- truck at 0 covers [-4, 4]. Covers playgrounds at -2, 2, 4.
All playgrounds covered. Minimum serving radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With serving radius 3:
- truck at 4 covers [1, 7]. Covers playgrounds 1, 5.
- truck at 11 covers [8, 14]. Covers playgrounds 10, 14.
- truck at 15 covers [12, 18]. Covers playground 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of playgrounds and trucks.
- The second line contains $n$ integers representing the coordinates of the playgrounds. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the trucks. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal serving radius $r$ required.

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
