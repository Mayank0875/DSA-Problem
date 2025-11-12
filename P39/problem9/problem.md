## Title

Binary Bloom

## Slug

binary-bloom

## Difficulty

Easy

## Description

Imagine a garden where each flower blooms with a certain intensity represented by an integer. As you walk along the garden path, for each flower you stand in front of, you look back (to your left) and want to know the intensity of the nearest previous flower that has a strictly higher intensity than the one you are currently observing. If all previous flowers are less intense or have equal intensity, or if it's the first flower, there is no such brighter bloom to the left. Your goal is to determine this brighter bloom's intensity for each position along the path.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Flower 0 (30): No previous flower. Output -1.
Flower 1 (60): Flower 0 (30) is less intense. Output -1.
Flower 2 (90): Flowers 0 (30), 1 (60) are less intense. Output -1.
Flower 3 (50): Flower 2 (90) is the nearest brighter bloom. Output 90.
Flower 4 (80): Flower 2 (90) is the nearest brighter bloom. Output 90.
Flower 5 (40): Flower 4 (80) is the nearest brighter bloom. Output 80.
Flower 6 (70): Flower 4 (80) is the nearest brighter bloom. Output 80.
Flower 7 (50): Flower 6 (70) is the nearest brighter bloom. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All flowers have equal intensity, so no strictly brighter previous bloom exists.

## Input Format

The first line contains a single integer n, the number of flowers.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the intensity of each flower.

## Output Format

Return array of integers. The i-th integer should be the intensity of the nearest flower j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array