## Title
Post Office Mail

## Slug
post-office-mail

## Difficulty
Medium

## Description
Residents live along a rural road. Mail carriers start from post offices and need to cover every home.

There are $n$ homes and $m$ post offices positioned at specific coordinates along a rural road.

The postmaster plans to establish a service range. All post offices will operate with the same delivery limit $r$. A post office at location $x$ with delivery limit $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every home must be covered by at least one post office.

Your task is to determine the **minimum non-negative integer delivery limit $r$** required to ensure that all $n$ homes are within the range of at least one post office.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
homes are at -2, 2, 4. post offices are at -3, 0.
With delivery limit 4:
- post office at -3 covers [-7, 1]. Covers home at -2.
- post office at 0 covers [-4, 4]. Covers homes at -2, 2, 4.
All homes covered. Minimum delivery limit is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With delivery limit 3:
- post office at 4 covers [1, 7]. Covers homes 1, 5.
- post office at 11 covers [8, 14]. Covers homes 10, 14.
- post office at 15 covers [12, 18]. Covers home 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of homes and post offices.
- The second line contains $n$ integers representing the coordinates of the homes. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the post offices. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal delivery limit $r$ required.

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
