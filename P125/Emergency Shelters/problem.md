## Title
Emergency Shelters

## Slug
emergency-shelters

## Difficulty
Medium

## Description
In a disaster simulation, citizens along a coastline need to reach safety bunkers. We must ensure every citizen is close enough to a bunker.

There are $n$ citizens and $m$ bunkers positioned at specific coordinates along a coastline road.

The coordinator plans to establish a service range. All bunkers will operate with the same travel distance $r$. A bunker at location $x$ with travel distance $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every citizen must be covered by at least one bunker.

Your task is to determine the **minimum non-negative integer travel distance $r$** required to ensure that all $n$ citizens are within the range of at least one bunker.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
citizens are at -2, 2, 4. bunkers are at -3, 0.
With travel distance 4:
- bunker at -3 covers [-7, 1]. Covers citizen at -2.
- bunker at 0 covers [-4, 4]. Covers citizens at -2, 2, 4.
All citizens covered. Minimum travel distance is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With travel distance 3:
- bunker at 4 covers [1, 7]. Covers citizens 1, 5.
- bunker at 11 covers [8, 14]. Covers citizens 10, 14.
- bunker at 15 covers [12, 18]. Covers citizen 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of citizens and bunkers.
- The second line contains $n$ integers representing the coordinates of the citizens. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the bunkers. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal travel distance $r$ required.

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
