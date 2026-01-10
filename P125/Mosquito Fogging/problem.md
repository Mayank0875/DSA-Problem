## Title
Mosquito Fogging

## Slug
mosquito-fogging

## Difficulty
Medium

## Description
Breeding pools in a swamp need to be reached by fogging machines.

There are $n$ pools and $m$ machines positioned at specific coordinates along a swamp edge.

The health officer plans to establish a service range. All machines will operate with the same fog radius $r$. A machine at location $x$ with fog radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every pool must be covered by at least one machine.

Your task is to determine the **minimum non-negative integer fog radius $r$** required to ensure that all $n$ pools are within the range of at least one machine.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
pools are at -2, 2, 4. machines are at -3, 0.
With fog radius 4:
- machine at -3 covers [-7, 1]. Covers pool at -2.
- machine at 0 covers [-4, 4]. Covers pools at -2, 2, 4.
All pools covered. Minimum fog radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With fog radius 3:
- machine at 4 covers [1, 7]. Covers pools 1, 5.
- machine at 11 covers [8, 14]. Covers pools 10, 14.
- machine at 15 covers [12, 18]. Covers pool 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of pools and machines.
- The second line contains $n$ integers representing the coordinates of the pools. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the machines. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal fog radius $r$ required.

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
