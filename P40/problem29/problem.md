## Title

Fractal Current

## Slug

fractal-current

## Difficulty

Easy

## Description

A researcher is studying the electrical current values observed at successive points in a fractal structure. For each point, they want to identify the current value of the nearest future point that exhibits a strictly higher current. This helps them understand the growth pattern of the current across the fractal. If no future point has a higher current (either because it is the last point or all subsequent points have lower or equal current), this should be noted. Can you calculate this for each point?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Point 0 (500): Next higher is 600 (Point 2). Output 600.
Point 1 (400): Next higher is 600 (Point 2). Output 600.
Point 2 (600): Next higher is 700 (Point 4). Output 700.
Point 3 (300): Next higher is 700 (Point 4). Output 700.
Point 4 (700): Next higher is 800 (Point 6). Output 800.
Point 5 (450): Next higher is 800 (Point 6). Output 800.
Point 6 (800): No future point is higher. Output -1.
Point 7 (500): No future point exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All current values are equal, so no future point has higher current.

## Input Format

The first line contains a single integer n, the number of points.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the current at each point.

## Output Format

Return array of integers. The i-th integer should be the current of the nearest point j > i such that a_j > a_i. If no such point exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array