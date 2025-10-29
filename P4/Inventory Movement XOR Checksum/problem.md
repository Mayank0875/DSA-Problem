## Title

Inventory Movement XOR Checksum

## Slug

inventory-movement-xor-checksum

## Difficulty

Easy

## Description

A warehouse manager tracks daily inventory changes (positive for additions, potentially encoded integers for movements) A₁, A₂, ..., Aₙ. To verify data integrity over K-day periods, they use a sliding window. For each window, a checksum is computed by XORing the daily change values within it. To obtain a final checksum for the entire tracking period, all window checksums are XORed together. Calculate this final inventory checksum.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Inventory change windows of size 3:
    •   [1, 2, 3] → Checksum (XOR) = 0
    •   [2, 3, 4] → Checksum (XOR) = 5
    •   [3, 4, 5] → Checksum (XOR) = 2

Final Checksum = 0 ^ 5 ^ 2 = 7

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

Final Checksum = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (number of days) and K (window size).
- The second line contains N space-separated integers — the daily inventory changes.

## Output Format

- Return a single integer — the final inventory checksum.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, logistics, bit manipulation