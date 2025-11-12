## Title

Quantum Cascade Energy Levels

## Slug

quantum-cascade

## Difficulty

Easy

## Description

Imagine a quantum cascade laser where electrons cascade through a series of energy levels of varying heights. As an electron reaches each level, it looks back (to lower indices) and wants to know the height of the nearest previous energy level that is strictly higher than the current one. If all earlier levels are lower or equal, or if it is the first level, there is no such higher level to the left. Your goal is to determine this higher level's energy for each position in the cascade.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Level 0 (30): No previous level. Output -1.
Level 1 (60): Level 0 (30) is lower. Output -1.
Level 2 (90): Levels 0 (30), 1 (60) are lower. Output -1.
Level 3 (50): Level 2 (90) is the nearest higher. Output 90.
Level 4 (80): Level 2 (90) is the nearest higher. Output 90.
Level 5 (40): Level 4 (80) is the nearest higher. Output 80.
Level 6 (70): Level 4 (80) is the nearest higher. Output 80.
Level 7 (50): Level 6 (70) is the nearest higher. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All levels have equal energy, so no strictly higher previous level exists.

## Input Format

The first line contains a single integer n, the number of energy levels.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the height of each level.

## Output Format

Return array of integers. The i-th integer should be the height of the nearest level j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array