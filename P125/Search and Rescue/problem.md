## Title
Search and Rescue

## Slug
search-and-rescue

## Difficulty
Medium

## Description
Lost hikers on a trail need to be found by rescue dogs starting from trailheads.

There are $n$ hikers and $m$ trailheads positioned at specific coordinates along a trail.

The rescue team plans to establish a service range. All trailheads will operate with the same sniffing range $r$. A trailhead at location $x$ with sniffing range $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every hiker must be covered by at least one trailhead.

Your task is to determine the **minimum non-negative integer sniffing range $r$** required to ensure that all $n$ hikers are within the range of at least one trailhead.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
hikers are at -2, 2, 4. trailheads are at -3, 0.
With sniffing range 4:
- trailhead at -3 covers [-7, 1]. Covers hiker at -2.
- trailhead at 0 covers [-4, 4]. Covers hikers at -2, 2, 4.
All hikers covered. Minimum sniffing range is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With sniffing range 3:
- trailhead at 4 covers [1, 7]. Covers hikers 1, 5.
- trailhead at 11 covers [8, 14]. Covers hikers 10, 14.
- trailhead at 15 covers [12, 18]. Covers hiker 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of hikers and trailheads.
- The second line contains $n$ integers representing the coordinates of the hikers. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the trailheads. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal sniffing range $r$ required.

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
