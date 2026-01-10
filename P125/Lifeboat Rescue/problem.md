## Title
Lifeboat Rescue

## Slug
lifeboat-rescue

## Difficulty
Medium

## Description
Swimmers are in distress along a straight beach. Lifeguard boats are stationed at intervals and need to reach everyone.

There are $n$ swimmers and $m$ boats positioned at specific coordinates along a shoreline.

The captain plans to establish a service range. All boats will operate with the same rescue radius $r$. A boat at location $x$ with rescue radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every swimmer must be covered by at least one boat.

Your task is to determine the **minimum non-negative integer rescue radius $r$** required to ensure that all $n$ swimmers are within the range of at least one boat.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
swimmers are at -2, 2, 4. boats are at -3, 0.
With rescue radius 4:
- boat at -3 covers [-7, 1]. Covers swimmer at -2.
- boat at 0 covers [-4, 4]. Covers swimmers at -2, 2, 4.
All swimmers covered. Minimum rescue radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With rescue radius 3:
- boat at 4 covers [1, 7]. Covers swimmers 1, 5.
- boat at 11 covers [8, 14]. Covers swimmers 10, 14.
- boat at 15 covers [12, 18]. Covers swimmer 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of swimmers and boats.
- The second line contains $n$ integers representing the coordinates of the swimmers. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the boats. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal rescue radius $r$ required.

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
