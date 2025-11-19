## Title

Fractal Current: Next Higher Intensity

## Slug

fractal-current-next-higher-intensity

## Difficulty

Easy

## Description

Scientists are studying the electrical current along a fractal structure. For each measurement point, they want to identify the current value at the nearest future point that exhibits a strictly higher intensity. This helps them understand how the current propagates and where peaks occur. If no future point has a higher current (either because it is the last point or all subsequent points have lower or equal intensity), this should be noted. Can you calculate this for each measurement point?

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

All current measurements are equal, so no future point has higher intensity.

## Input Format

The first line contains a single integer n, the number of measurement points.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the current intensity at each point.

## Output Format

Return array of integers. The i-th integer should be the intensity of the nearest point j > i such that a_j > a_i. If no such point exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array