## Title

The Obsidian Key

## Slug

the-obsidian-key

## Difficulty

Easy

## Description

You are an adventurer navigating a corridor of ancient chambers, each infused with a distinct magical power level. As you stand in front of a chamber, you glance back (to your left) to discover the nearest previous chamber whose power level is **strictly greater** than the one you are currently in front of. If all earlier chambers have lower or equal power, or if you are at the very first chamber, there is no such more powerful chamber to the left. Your task is to determine the power level of this nearest, more powerful chamber for every position along the corridor.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Chamber 0 (30): No previous chamber. Output -1.  
Chamber 1 (60): Chamber 0 (30) is weaker. Output -1.  
Chamber 2 (90): Chambers 0 (30), 1 (60) are weaker. Output -1.  
Chamber 3 (50): Chamber 2 (90) is the nearest stronger. Output 90.  
Chamber 4 (80): Chamber 2 (90) is the nearest stronger. Output 90.  
Chamber 5 (40): Chamber 4 (80) is the nearest stronger. Output 80.  
Chamber 6 (70): Chamber 4 (80) is the nearest stronger. Output 80.  
Chamber 7 (50): Chamber 6 (70) is the nearest stronger. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All chambers have equal power, so no strictly stronger previous chamber exists.

## Input Format

The first line contains a single integer n, the number of chambers.  
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the power level of each chamber.

## Output Format

Return array of integers. The i-th integer should be the power level of the nearest chamber j < i such that h_j > h_i. If no such chamber exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array