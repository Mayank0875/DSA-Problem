## Title
Vaccination Drive

## Slug
vaccination-drive

## Difficulty
Medium

## Description
Remote hamlets along a river need access to mobile vaccination boats.

There are $n$ hamlets and $m$ boats positioned at specific coordinates along a river bank.

The doctor plans to establish a service range. All boats will operate with the same access radius $r$. A boat at location $x$ with access radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every hamlet must be covered by at least one boat.

Your task is to determine the **minimum non-negative integer access radius $r$** required to ensure that all $n$ hamlets are within the range of at least one boat.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
hamlets are at -2, 2, 4. boats are at -3, 0.
With access radius 4:
- boat at -3 covers [-7, 1]. Covers hamlet at -2.
- boat at 0 covers [-4, 4]. Covers hamlets at -2, 2, 4.
All hamlets covered. Minimum access radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With access radius 3:
- boat at 4 covers [1, 7]. Covers hamlets 1, 5.
- boat at 11 covers [8, 14]. Covers hamlets 10, 14.
- boat at 15 covers [12, 18]. Covers hamlet 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of hamlets and boats.
- The second line contains $n$ integers representing the coordinates of the hamlets. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the boats. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal access radius $r$ required.

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
