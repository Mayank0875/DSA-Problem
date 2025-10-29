## Title

Artifact Layer XOR Checksum

## Slug

artifact-layer-xor-checksum

## Difficulty

Easy

## Description

An archaeologist analyzes numerical data A₁, A₂, ..., Aₙ representing characteristics of artifact layers found at a dig site. To check for data consistency within K consecutive layers (a window), they calculate a checksum by XORing the characteristic values in each window. To generate a single checksum value representing the entire sequence of layers, all the window checksums are XORed together. Compute this final checksum value.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Layer data windows of size 3:
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

- The first line contains two integers N (number of layers) and K (window size).
- The second line contains N space-separated integers — the characteristic values.

## Output Format

- Return a single integer — the final checksum value.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, data analysis, bit manipulation