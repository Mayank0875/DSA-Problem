## Title

Next Higher Code Depth

## Slug

next-higher-code-depth

## Difficulty

Easy

## Description

A programmer is exploring the **Code Abyss**, analyzing the depth levels of a sequence of code modules to plan the next steps in refactoring. For each module, they want to identify the depth value of the nearest future module that has a strictly higher depth. This helps them understand how complexity evolves or spot particularly deep sections. If no future module has a higher depth (either because it is the last module or all subsequent modules have lower or equal depth), this should be noted. Can you calculate this for each module?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Module 0 (500): Next higher is 600 (Module 2). Output 600.  
Module 1 (400): Next higher is 600 (Module 2). Output 600.  
Module 2 (600): Next higher is 700 (Module 4). Output 700.  
Module 3 (300): Next higher is 700 (Module 4). Output 700.  
Module 4 (700): Next higher is 800 (Module 6). Output 800.  
Module 5 (450): Next higher is 800 (Module 6). Output 800.  
Module 6 (800): No future module is higher. Output -1.  
Module 7 (500): No future module exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All depths are equal, so no future module has a higher depth.

## Input Format

The first line contains a single integer n, the number of modules.  
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the depth of each module.

## Output Format

Return array of integers. The i‑th integer should be the depth of the nearest module j > i such that a_j > a_i. If no such module exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array