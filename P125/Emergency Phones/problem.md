## Title
Emergency Phones

## Slug
emergency-phones

## Difficulty
Medium

## Description
Breakdown spots on a bridge must be near SOS phones.

There are $n$ breakdown spots and $m$ phones positioned at specific coordinates along a bridge.

The safety officer plans to establish a service range. All phones will operate with the same access distance $r$. A phone at location $x$ with access distance $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every breakdown spot must be covered by at least one phone.

Your task is to determine the **minimum non-negative integer access distance $r$** required to ensure that all $n$ breakdown spots are within the range of at least one phone.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
breakdown spots are at -2, 2, 4. phones are at -3, 0.
With access distance 4:
- phone at -3 covers [-7, 1]. Covers breakdown spot at -2.
- phone at 0 covers [-4, 4]. Covers breakdown spots at -2, 2, 4.
All breakdown spots covered. Minimum access distance is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With access distance 3:
- phone at 4 covers [1, 7]. Covers breakdown spots 1, 5.
- phone at 11 covers [8, 14]. Covers breakdown spots 10, 14.
- phone at 15 covers [12, 18]. Covers breakdown spot 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of breakdown spots and phones.
- The second line contains $n$ integers representing the coordinates of the breakdown spots. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the phones. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal access distance $r$ required.

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
