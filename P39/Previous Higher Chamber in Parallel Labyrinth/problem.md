## Title

Previous Higher Chamber in Parallel Labyrinth

## Slug

previous-higher-chamber-parallel-labyrinth

## Difficulty

Easy

## Description

Imagine navigating a parallel labyrinth composed of a sequence of chambers, each with its own height. As you stand in front of a chamber, you glance back (to the left) along the path you have already taken and want to know the height of the nearest chamber that is strictly taller than the one you are currently in front of. If all previously visited chambers are shorter or of equal height, or if it is the first chamber, there is no such taller chamber to the left. Your goal is to determine this taller chamber's height for each position along the labyrinth.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Chamber 0 (30): No previous chamber. Output -1.
Chamber 1 (60): Chamber 0 (30) is shorter. Output -1.
Chamber 2 (90): Chambers 0 (30), 1 (60) are shorter. Output -1.
Chamber 3 (50): Chamber 2 (90) is the nearest taller. Output 90.
Chamber 4 (80): Chamber 2 (90) is the nearest taller. Output 90.
Chamber 5 (40): Chamber 4 (80) is the nearest taller. Output 80.
Chamber 6 (70): Chamber 4 (80) is the nearest taller. Output 80.
Chamber 7 (50): Chamber 6 (70) is the nearest taller. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All chambers are equal, so no strictly taller previous chamber exists.

## Input Format

The first line contains a single integer n, the number of chambers.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the height of each chamber.

## Output Format

Return array of integers. The i-th integer should be the height of the nearest chamber j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array