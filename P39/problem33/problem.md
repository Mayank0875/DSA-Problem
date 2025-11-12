## Title

Phantom Recursion

## Slug

phantom-recursion

## Difficulty

Easy

## Description

Imagine a mysterious program that invokes a chain of recursive calls, each call carrying a certain “energy” value. As you examine each call in the sequence, you look back into the call stack (to the earlier calls) and want to know the energy of the nearest previous call that has a strictly higher energy than the current one. If all earlier calls have equal or lower energy, or if it is the first call, there is no such higher‑energy call to the left. Your task is to determine this higher energy value for every position in the recursion chain.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Call 0 (30): No previous call. Output -1.  
Call 1 (60): Call 0 (30) is lower. Output -1.  
Call 2 (90): Calls 0 (30), 1 (60) are lower. Output -1.  
Call 3 (50): Call 2 (90) is the nearest higher. Output 90.  
Call 4 (80): Call 2 (90) is the nearest higher. Output 90.  
Call 5 (40): Call 4 (80) is the nearest higher. Output 80.  
Call 6 (70): Call 4 (80) is the nearest higher. Output 80.  
Call 7 (50): Call 6 (70) is the nearest higher. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All calls have equal energy, so no strictly higher previous call exists.

## Input Format

The first line contains a single integer n, the number of recursive calls.  
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the energy of each call.

## Output Format

Return array of integers. The i-th integer should be the energy of the nearest call j < i such that h_j > h_i. If no such call exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array