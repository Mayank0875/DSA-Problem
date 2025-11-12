## Title

Fractal Current

## Slug

fractal-current

## Difficulty

Easy

## Description

Imagine observing a river where the speed of the current varies at successive measurement points. At each point you look upstream (to your left) and want to know the speed of the nearest point that has a strictly stronger current than the one you are currently measuring. If all upstream points are slower or have equal speed, or if it is the first measurement point, there is no such stronger current upstream. Your goal is to determine this stronger current's speed for each position along the river.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Point 0 (30): No previous point. Output -1.  
Point 1 (60): Point 0 (30) is slower. Output -1.  
Point 2 (90): Points 0 (30), 1 (60) are slower. Output -1.  
Point 3 (50): Point 2 (90) is the nearest stronger. Output 90.  
Point 4 (80): Point 2 (90) is the nearest stronger. Output 90.  
Point 5 (40): Point 4 (80) is the nearest stronger. Output 80.  
Point 6 (70): Point 4 (80) is the nearest stronger. Output 80.  
Point 7 (50): Point 6 (70) is the nearest stronger. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All points have equal speed, so no strictly stronger upstream point exists.

## Input Format

The first line contains a single integer n, the number of measurement points.  
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the speed of the current at each point.

## Output Format

Return array of integers. The i-th integer should be the speed of the nearest point j < i such that h_j > h_i. If no such point exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array