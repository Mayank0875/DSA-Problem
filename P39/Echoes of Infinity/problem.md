## Title

Echoes of Infinity

## Slug

echoes-of-infinity

## Difficulty

Easy

## Description

Imagine traveling through an endless corridor of resonating chambers, each emitting a tone of a certain intensity. As you stand in front of each chamber, you look back (to your left) and want to know the intensity of the nearest chamber that is strictly louder than the one you are currently in front of. If all previous chambers are quieter or of equal intensity, or if it's the first chamber, there's no such louder chamber to the left. Your goal is to determine this louder chamber's intensity for each position along the corridor.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Building 0 (30): No previous building. Output -1.
Building 1 (60): Building 0 (30) is shorter. Output -1.
Building 2 (90): Buildings 0 (30), 1 (60) are shorter. Output -1.
Building 3 (50): Building 2 (90) is the nearest taller. Output 90.
Building 4 (80): Building 2 (90) is the nearest taller. Output 90.
Building 5 (40): Building 4 (80) is the nearest taller. Output 80.
Building 6 (70): Building 4 (80) is the nearest taller. Output 80.
Building 7 (50): Building 6 (70) is the nearest taller. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All Building are equal, so no strictly taller previous building exists.

## Input Format

The first line contains a single integer n, the number of buildings.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the height of each building.

## Output Format

Return array of integers. The i-th integer should be the height of the nearest building j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array