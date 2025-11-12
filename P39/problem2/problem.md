## Title

Shadow Spectrum: Nearest Brighter Shadow

## Slug

shadow-spectrum-nearest-brighter-shadow

## Difficulty

Easy

## Description

Imagine traversing a realm of shifting shadows, each cast with a different intensity on the ground. As you stand at a point and observe the shadow behind you (to your left), you want to know the intensity of the nearest previous shadow that is strictly brighter than the one you are currently standing in. If all earlier shadows are dimmer or of equal intensity, or if you are at the very first point, there is no such brighter shadow to the left. Your goal is to determine this brighter shadow's intensity for each position along the path.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Shadow 0 (30): No previous shadow. Output -1.
Shadow 1 (60): Shadow 0 (30) is dimmer. Output -1.
Shadow 2 (90): Shadows 0 (30), 1 (60) are dimmer. Output -1.
Shadow 3 (50): Shadow 2 (90) is the nearest brighter. Output 90.
Shadow 4 (80): Shadow 2 (90) is the nearest brighter. Output 90.
Shadow 5 (40): Shadow 4 (80) is the nearest brighter. Output 80.
Shadow 6 (70): Shadow 4 (80) is the nearest brighter. Output 80.
Shadow 7 (50): Shadow 6 (70) is the nearest brighter. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All shadows have equal intensity, so no strictly brighter previous shadow exists.

## Input Format

The first line contains a single integer n, the number of shadows.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the intensity of each shadow.

## Output Format

Return array of integers. The i-th integer should be the intensity of the nearest shadow j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array