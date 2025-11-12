## Title

Next Higher Paradox Value

## Slug

next-higher-paradox-value

## Difficulty

Easy

## Description

A philosopher is analyzing a sequence of paradoxical statements, each assigned a numeric paradox strength. For each statement, they want to identify the paradox strength of the nearest future statement that has a strictly higher strength. This helps them understand how paradoxes intensify over time. If no future statement has a higher strength (either because it is the last statement or all subsequent statements have lower or equal strength), this should be noted. Can you calculate this for each statement?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Statement 0 (500): Next higher is 600 (Statement 2). Output 600.
Statement 1 (400): Next higher is 600 (Statement 2). Output 600.
Statement 2 (600): Next higher is 700 (Statement 4). Output 700.
Statement 3 (300): Next higher is 700 (Statement 4). Output 700.
Statement 4 (700): Next higher is 800 (Statement 6). Output 800.
Statement 5 (450): Next higher is 800 (Statement 6). Output 800.
Statement 6 (800): No future statement is higher. Output -1.
Statement 7 (500): No future statement exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All paradox strengths are equal, so no future statement has a higher strength.

## Input Format

The first line contains a single integer n, the number of statements.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the paradox strength for each statement.

## Output Format

Return array of integers. The i-th integer should be the strength of the nearest statement j > i such that a_j > a_i. If no such statement exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array