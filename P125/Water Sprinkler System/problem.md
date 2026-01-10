## Title
Water Sprinkler System

## Slug
water-sprinkler-system

## Difficulty
Medium

## Description
A gardener is setting up irrigation for a flowerbed. Specific plants need water, provided by rotating sprinklers.

There are $n$ plants and $m$ sprinklers positioned at specific coordinates along a garden strip.

The gardener plans to establish a service range. All sprinklers will operate with the same spray radius $r$. A sprinkler at location $x$ with spray radius $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every plant must be covered by at least one sprinkler.

Your task is to determine the **minimum non-negative integer spray radius $r$** required to ensure that all $n$ plants are within the range of at least one sprinkler.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
plants are at -2, 2, 4. sprinklers are at -3, 0.
With spray radius 4:
- sprinkler at -3 covers [-7, 1]. Covers plant at -2.
- sprinkler at 0 covers [-4, 4]. Covers plants at -2, 2, 4.
All plants covered. Minimum spray radius is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With spray radius 3:
- sprinkler at 4 covers [1, 7]. Covers plants 1, 5.
- sprinkler at 11 covers [8, 14]. Covers plants 10, 14.
- sprinkler at 15 covers [12, 18]. Covers plant 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of plants and sprinklers.
- The second line contains $n$ integers representing the coordinates of the plants. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the sprinklers. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal spray radius $r$ required.

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
