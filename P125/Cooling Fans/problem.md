## Title
Cooling Fans

## Slug
cooling-fans

## Difficulty
Medium

## Description
Overheating servers in a row need cooling from industrial fans placed on the floor.

There are $n$ servers and $m$ fans positioned at specific coordinates along a server aisle.

The technician plans to establish a service range. All fans will operate with the same airflow range $r$. A fan at location $x$ with airflow range $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every server must be covered by at least one fan.

Your task is to determine the **minimum non-negative integer airflow range $r$** required to ensure that all $n$ servers are within the range of at least one fan.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
servers are at -2, 2, 4. fans are at -3, 0.
With airflow range 4:
- fan at -3 covers [-7, 1]. Covers server at -2.
- fan at 0 covers [-4, 4]. Covers servers at -2, 2, 4.
All servers covered. Minimum airflow range is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With airflow range 3:
- fan at 4 covers [1, 7]. Covers servers 1, 5.
- fan at 11 covers [8, 14]. Covers servers 10, 14.
- fan at 15 covers [12, 18]. Covers server 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of servers and fans.
- The second line contains $n$ integers representing the coordinates of the servers. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the fans. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal airflow range $r$ required.

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
