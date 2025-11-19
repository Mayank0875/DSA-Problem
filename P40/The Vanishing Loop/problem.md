## Title

The Vanishing Loop

## Slug

the-vanishing-loop

## Difficulty

Easy

## Description

In an ancient library, a mysterious loop of scrolls is arranged in a line. Each scroll bears a number. When a scroll is examined, the next scroll that **vanishes** after it reveals a larger number than the one on the current scroll. For every scroll, you must determine the number on the nearest later scroll that vanishes with a strictly higher value. If there is no such later scroll (either because it is the last scroll or all subsequent scrolls have lower or equal numbers), record this fact. Compute this for each scroll in the sequence.

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Scroll 0 (500): The next vanishing scroll with a higher number is 600 (Scroll 2). Output 600.  
Scroll 1 (400): The next vanishing scroll with a higher number is 600 (Scroll 2). Output 600.  
Scroll 2 (600): The next vanishing scroll with a higher number is 700 (Scroll 4). Output 700.  
Scroll 3 (300): The next vanishing scroll with a higher number is 700 (Scroll 4). Output 700.  
Scroll 4 (700): The next vanishing scroll with a higher number is 800 (Scroll 6). Output 800.  
Scroll 5 (450): The next vanishing scroll with a higher number is 800 (Scroll 6). Output 800.  
Scroll 6 (800): No later scroll vanishes with a higher number. Output -1.  
Scroll 7 (500): No later scroll exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All numbers are equal, so no later scroll vanishes with a higher number.

## Input Format

The first line contains a single integer n, the number of scrolls.  
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the number on each scroll.

## Output Format

Return array of integers. The i‑th integer should be the number on the nearest scroll j > i such that a_j > a_i. If no such scroll exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array