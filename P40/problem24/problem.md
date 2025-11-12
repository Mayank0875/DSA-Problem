## Title

Memory Fracture: Next Higher Signal

## Slug

memory-fracture-next-higher-signal

## Difficulty

Easy

## Description

In a fractured memory system, each cell stores a signal strength value. For every cell, we need to determine the signal strength of the nearest subsequent cell that contains a strictly higher value. This information helps in diagnosing the propagation of stronger signals through the damaged memory. If there is no later cell with a higher signal (either because it is the last cell or all following cells have lower or equal values), this should be indicated. Compute this for each cell.

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Cell 0 (500): Next higher is 600 (Cell 2). Output 600.
Cell 1 (400): Next higher is 600 (Cell 2). Output 600.
Cell 2 (600): Next higher is 700 (Cell 4). Output 700.
Cell 3 (300): Next higher is 700 (Cell 4). Output 700.
Cell 4 (700): Next higher is 800 (Cell 6). Output 800.
Cell 5 (450): Next higher is 800 (Cell 6). Output 800.
Cell 6 (800): No later cell is higher. Output -1.
Cell 7 (500): No later cell exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All signal strengths are equal, so no later cell has a higher value.

## Input Format

The first line contains a single integer n, the number of memory cells.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the signal strength stored in each cell.

## Output Format

Return array of integers. The i-th integer should be the signal strength of the nearest cell j > i such that a_j > a_i. If no such cell exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array