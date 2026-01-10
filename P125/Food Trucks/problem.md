## Title
Food Trucks

## Slug
food-trucks

## Difficulty
Medium

## Description
Office buildings on a busy street have hungry workers. Food trucks park at designated spots.

There are $n$ buildings and $m$ food trucks positioned at specific coordinates along a street.

The vendor plans to establish a service range. All food trucks will operate with the same walking limit $r$. A food truck at location $x$ with walking limit $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every building must be covered by at least one food truck.

Your task is to determine the **minimum non-negative integer walking limit $r$** required to ensure that all $n$ buildings are within the range of at least one food truck.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
buildings are at -2, 2, 4. food trucks are at -3, 0.
With walking limit 4:
- food truck at -3 covers [-7, 1]. Covers building at -2.
- food truck at 0 covers [-4, 4]. Covers buildings at -2, 2, 4.
All buildings covered. Minimum walking limit is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With walking limit 3:
- food truck at 4 covers [1, 7]. Covers buildings 1, 5.
- food truck at 11 covers [8, 14]. Covers buildings 10, 14.
- food truck at 15 covers [12, 18]. Covers building 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of buildings and food trucks.
- The second line contains $n$ integers representing the coordinates of the buildings. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the food trucks. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal walking limit $r$ required.

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
