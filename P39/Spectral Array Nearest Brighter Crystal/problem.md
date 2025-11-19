## Title

Spectral Array: Nearest Brighter Crystal

## Slug

spectral-array-nearest-brighter-crystal

## Difficulty

Easy

## Description

Imagine a line of magical crystals, each radiating a certain intensity. As you examine each crystal in order, you look back (to the left) and want to know the intensity of the nearest crystal that shines **strictly brighter** than the one you are currently observing. If all previous crystals are dimmer or of equal intensity, or if it is the first crystal, there is no such brighter crystal to the left. Your goal is to determine this brighter crystal's intensity for every position in the line.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Crystal 0 (30): No previous crystal. Output -1.  
Crystal 1 (60): Crystal 0 (30) is dimmer. Output -1.  
Crystal 2 (90): Crystals 0 (30), 1 (60) are dimmer. Output -1.  
Crystal 3 (50): Crystal 2 (90) is the nearest brighter. Output 90.  
Crystal 4 (80): Crystal 2 (90) is the nearest brighter. Output 90.  
Crystal 5 (40): Crystal 4 (80) is the nearest brighter. Output 80.  
Crystal 6 (70): Crystal 4 (80) is the nearest brighter. Output 80.  
Crystal 7 (50): Crystal 6 (70) is the nearest brighter. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All crystals emit the same intensity, so no strictly brighter previous crystal exists.

## Input Format

The first line contains a single integer n, the number of crystals.  
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the intensity of each crystal.

## Output Format

Return array of integers. The i-th integer should be the intensity of the nearest crystal j < i such that h_j > h_i. If no such crystal exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array