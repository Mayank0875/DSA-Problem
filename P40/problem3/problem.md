## Title

Recursive Tide

## Slug

recursive-tide

## Difficulty

Easy

## Description

A coastal research team is analyzing a sequence of recorded tide heights to understand the ocean's behavior. For each recorded tide, they want to identify the height of the nearest future tide that is strictly higher. This helps them predict rising water levels and detect significant surges. If no future tide is higher (either because it is the last measurement or all subsequent tides are lower or equal), this should be noted. Can you calculate this for each tide measurement?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Concert 0 (500): Next higher is 600 (Concert 2). Output 600.
Concert 1 (400): Next higher is 600 (Concert 2). Output 600.
Concert 2 (600): Next higher is 700 (Concert 4). Output 700.
Concert 3 (300): Next higher is 700 (Concert 4). Output 700.
Concert 4 (700): Next higher is 800 (Concert 6). Output 800.
Concert 5 (450): Next higher is 800 (Concert 6). Output 800.
Concert 6 (800): No future concert is higher. Output -1.
Concert 7 (500): No future concert exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All Attendance are equal, so no future concert has higher attendance.

## Input Format

The first line contains a single integer n, the number of concerts.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the audience attendance for each concert.

## Output Format

Return array of integers. The i-th integer should be the attendance of the nearest concert j > i such that a_j > a_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array