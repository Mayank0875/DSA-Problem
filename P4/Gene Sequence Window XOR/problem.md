## Title

Gene Sequence Window XOR

## Slug

gene-sequence-window-xor

## Difficulty

Easy

## Description

A biologist is studying a gene sequence represented numerically as A₁, A₂, ..., Aₙ. They are interested in identifying patterns within fixed-length segments (windows) of size K. For each segment, a characteristic value is calculated by XORing all the numerical representations within that window. To summarize the pattern across the entire sequence, these characteristic values from all windows are XORed together. Calculate the final summary value for the given gene sequence.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Sequence windows of size 3:
    •   [1, 2, 3] → Characteristic Value (XOR) = 0
    •   [2, 3, 4] → Characteristic Value (XOR) = 5
    •   [3, 4, 5] → Characteristic Value (XOR) = 2

Final Summary Value = 0 ^ 5 ^ 2 = 7

### 2

#### Input

4 2
[5, 1, 3, 2]

#### Output

7

#### Explanation

Windows:
    •   [5, 1] → XOR = 4
    •   [1, 3] → XOR = 2
    •   [3, 2] → XOR = 1

Final Summary Value = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (sequence length) and K (window size).
- The second line contains N space-separated integers — the numerical gene representations.

## Output Format

- Return a single integer — the final summary value.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, biology, bit manipulation