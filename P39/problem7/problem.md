## Title

Code Abyss: Previous Taller Function Call

## Slug

code-abyss-previous-taller-function-call

## Difficulty

Easy

## Description

Imagine navigating the depths of the Code Abyss, where each line of code has an associated complexity rating. As you examine each line, you look back (to earlier lines) and want to know the complexity of the nearest previous line that is strictly more complex than the current one. If all earlier lines are less complex or have equal complexity, or if it's the first line, there is no such more complex line to the left. Your goal is to determine this higher complexity value for each position in the code sequence.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Line 0 (30): No previous line. Output -1.
Line 1 (60): Line 0 (30) is less complex. Output -1.
Line 2 (90): Lines 0 (30), 1 (60) are less complex. Output -1.
Line 3 (50): Line 2 (90) is the nearest more complex. Output 90.
Line 4 (80): Line 2 (90) is the nearest more complex. Output 90.
Line 5 (40): Line 4 (80) is the nearest more complex. Output 80.
Line 6 (70): Line 4 (80) is the nearest more complex. Output 80.
Line 7 (50): Line 6 (70) is the nearest more complex. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All lines have equal complexity, so no strictly more complex previous line exists.

## Input Format

The first line contains a single integer n, the number of code lines.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the complexity of each line.

## Output Format

Return array of integers. The i-th integer should be the complexity of the nearest line j < i such that h_j > h_i. If no such line exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array