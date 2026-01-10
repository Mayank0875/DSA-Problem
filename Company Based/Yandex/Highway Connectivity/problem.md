## Title

Highway Connectivity

## Slug

highway-connectivity

## Difficulty

Medium

## Description

A government agency is upgrading the digital infrastructure along a long, straight highway. There are $n$ bus stops and $m$ Wi-Fi tower locations positioned at specific coordinates along this highway.

The agency plans to install Wi-Fi transmitters at all $m$ tower locations. All transmitters will operate with the same signal radius $r$. A tower at location $x$ with radius $r$ provides coverage to the interval $[x - r, x + r]$.

For the upgrade to be successful, every bus stop must be covered by at least one Wi-Fi tower.

Your task is to determine the minimum non-negative integer radius $r$ required to ensure that all $n$ bus stops are within the range of at least one tower.

## Examples

### 1

#### Input

3 2
-2 2 4
-3 0

#### Output

4

#### Explanation

Bus stops are at -2, 2, 4. Towers are at -3, 0.
With radius 4:
- Tower at -3 covers [-7, 1]. Covers bus stop at -2.
- Tower at 0 covers [-4, 4]. Covers bus stops at -2, 2, 4.
All stops covered. Minimum radius is 4.
    
### 2

#### Input

5 3
1 5 10 14 17
4 11 15

#### Output

3

#### Explanation

With radius 3:
- Tower at 4 covers [1, 7]. Covers stops 1, 5.
- Tower at 11 covers [8, 14]. Covers stops 10, 14.
- Tower at 15 covers [12, 18]. Covers stop 17.

## Input Format  

- The first line contains two integers $n$ and $m$ — the number of bus stops and towers.
- The second line contains $n$ integers $a_1, a_2, \dots, a_n$ — the coordinates of the bus stops. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers $b_1, b_2, \dots, b_m$ — the coordinates of the towers. The coordinates are sorted in non-decreasing order.

## Output Format  

- Return a single integer — the minimal radius $r$ required.
  

## Constraints  

- 1 ≤ n, m ≤ 1e5
- -1e9 ≤ a_i, b_i ≤ 1e9
- The input arrays are sorted in non-decreasing order.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, two-pointers, array