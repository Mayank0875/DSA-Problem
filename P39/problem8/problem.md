## Title

Forgotten Bit

## Slug

forgotten-bit

## Difficulty

Easy

## Description

Imagine a sequence of memory cells arranged in a line, each holding an integer value that represents a certain bit‑pattern strength. As you inspect each cell from left to right, you look back (to the previous cells) and want to know the value of the nearest cell that contains a strictly larger bit‑pattern than the current one. If all earlier cells are weaker or equal, or if you are at the very first cell, there is no such stronger previous cell. Your task is to determine this stronger cell's value for every position in the sequence.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Cell 0 (30): No previous cell. Output -1.
Cell 1 (60): Cell 0 (30) is weaker. Output -1.
Cell 2 (90): Cells 0 (30), 1 (60) are weaker. Output -1.
Cell 3 (50): Cell 2 (90) is the nearest stronger. Output 90.
Cell 4 (80): Cell 2 (90) is the nearest stronger. Output 90.
Cell 5 (40): Cell 4 (80) is the nearest stronger. Output 80.
Cell 6 (70): Cell 4 (80) is the nearest stronger. Output 80.
Cell 7 (50): Cell 6 (70) is the nearest stronger. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All cells have equal strength, so no strictly stronger previous cell exists.

## Input Format

The first line contains a single integer n, the number of memory cells.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the value stored in each cell.

## Output Format

Return array of integers. The i-th integer should be the value of the nearest cell j < i such that h_j > h_i. If no such cell exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array