## Title

Temperature Fluctuation XOR Index

## Slug

temperature-fluctuation-xor-index

## Difficulty

Easy

## Description

A meteorologist is studying a sequence of daily average temperatures A₁, A₂, ..., Aₙ. To analyze short-term temperature swings, they use a sliding window of size K. For each K-day period, an index is calculated by XORing the temperatures within that window. To get a single measure summarizing these swings over the whole period, all the calculated indices are XORed together. Compute this final temperature fluctuation index.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Temperature windows of size 3:
    •   [1, 2, 3] → Index (XOR) = 0
    •   [2, 3, 4] → Index (XOR) = 5
    •   [3, 4, 5] → Index (XOR) = 2

Final Fluctuation Index = 0 ^ 5 ^ 2 = 7

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

Final Fluctuation Index = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (number of days) and K (window size).
- The second line contains N space-separated integers — the daily average temperatures.

## Output Format

- Return a single integer — the final temperature fluctuation index.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9 (Using integers for simplicity)

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, data analysis, bit manipulation