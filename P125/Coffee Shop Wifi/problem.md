## Title
Coffee Shop Wifi

## Slug
coffee-shop-wifi

## Difficulty
Medium

## Description
Customers sitting at tables along a wall need Wi-Fi. Routers are placed at specific outlets.

There are $n$ tables and $m$ routers positioned at specific coordinates along a cafe wall.

The barista plans to establish a service range. All routers will operate with the same signal reach $r$. A router at location $x$ with signal reach $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every table must be covered by at least one router.

Your task is to determine the **minimum non-negative integer signal reach $r$** required to ensure that all $n$ tables are within the range of at least one router.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
tables are at -2, 2, 4. routers are at -3, 0.
With signal reach 4:
- router at -3 covers [-7, 1]. Covers table at -2.
- router at 0 covers [-4, 4]. Covers tables at -2, 2, 4.
All tables covered. Minimum signal reach is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With signal reach 3:
- router at 4 covers [1, 7]. Covers tables 1, 5.
- router at 11 covers [8, 14]. Covers tables 10, 14.
- router at 15 covers [12, 18]. Covers table 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of tables and routers.
- The second line contains $n$ integers representing the coordinates of the tables. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the routers. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal signal reach $r$ required.

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
