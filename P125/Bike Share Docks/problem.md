## Title
Bike Share Docks

## Slug
bike-share-docks

## Difficulty
Medium

## Description
Tourist spots along a river need bike share docks nearby.

There are $n$ spots and $m$ docks positioned at specific coordinates along a river path.

The tourist plans to establish a service range. All docks will operate with the same riding radius $r$. A dock at location $x$ with riding radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every spot must be covered by at least one dock.

Your task is to determine the **minimum non-negative integer riding radius $r$** required to ensure that all $n$ spots are within the range of at least one dock.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
spots are at -2, 2, 4. docks are at -3, 0.
With riding radius 4:
- dock at -3 covers [-7, 1]. Covers spot at -2.
- dock at 0 covers [-4, 4]. Covers spots at -2, 2, 4.
All spots covered. Minimum riding radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With riding radius 3:
- dock at 4 covers [1, 7]. Covers spots 1, 5.
- dock at 11 covers [8, 14]. Covers spots 10, 14.
- dock at 15 covers [12, 18]. Covers spot 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of spots and docks.
- The second line contains $n$ integers representing the coordinates of the spots. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the docks. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal riding radius $r$ required.

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
