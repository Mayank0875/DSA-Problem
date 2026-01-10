## Title
Refugee Aid

## Slug
refugee-aid

## Difficulty
Medium

## Description
Refugee tents are pitched along a border. Supply trucks stop at checkpoints to distribute food.

There are $n$ tents and $m$ trucks positioned at specific coordinates along a border line.

The aid worker plans to establish a service range. All trucks will operate with the same distribution radius $r$. A truck at location $x$ with distribution radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every tent must be covered by at least one truck.

Your task is to determine the **minimum non-negative integer distribution radius $r$** required to ensure that all $n$ tents are within the range of at least one truck.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
tents are at -2, 2, 4. trucks are at -3, 0.
With distribution radius 4:
- truck at -3 covers [-7, 1]. Covers tent at -2.
- truck at 0 covers [-4, 4]. Covers tents at -2, 2, 4.
All tents covered. Minimum distribution radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With distribution radius 3:
- truck at 4 covers [1, 7]. Covers tents 1, 5.
- truck at 11 covers [8, 14]. Covers tents 10, 14.
- truck at 15 covers [12, 18]. Covers tent 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of tents and trucks.
- The second line contains $n$ integers representing the coordinates of the tents. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the trucks. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal distribution radius $r$ required.

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
