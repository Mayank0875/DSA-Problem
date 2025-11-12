## Title

Previous Higher Tide Level

## Slug

previous-higher-tide-level

## Difficulty

Easy

## Description

Imagine walking along a coastline where the water level (tide) varies at different points. As you stand at each point, you look back (to your left) and want to know the height of the nearest previous point where the tide was strictly higher than the current one. If all previous tide levels are lower or equal, or if it's the first point, there is no such higher tide to the left. Your goal is to determine this higher tide's height for each position along the shore.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Point 0 (30): No previous point. Output -1.
Point 1 (60): Point 0 (30) is lower. Output -1.
Point 2 (90): Points 0 (30), 1 (60) are lower. Output -1.
Point 3 (50): Point 2 (90) is the nearest higher. Output 90.
Point 4 (80): Point 2 (90) is the nearest higher. Output 90.
Point 5 (40): Point 4 (80) is the nearest higher. Output 80.
Point 6 (70): Point 4 (80) is the nearest higher. Output 80.
Point 7 (50): Point 6 (70) is the nearest higher. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All tide levels are equal, so no strictly higher previous tide exists.

## Input Format

The first line contains a single integer n, the number of points.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the tide height at each point.

## Output Format

Return array of integers. The i-th integer should be the height of the nearest point j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array