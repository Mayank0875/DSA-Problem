## Title

Signal Integrity Check

## Slug

signal-integrity-check

## Difficulty

Easy

## Description

Professor Elena is analyzing signal transmissions. The signal is represented as a sequence of integer values A₁, A₂, ..., Aₙ. To check for consistency, she needs to examine segments of the signal using a sliding window of size K. For each window, she calculates a checksum by XORing all values within that window. Finally, to get an overall integrity value for the transmission, she XORs together all the individual window checksums. Help Professor Elena compute this final integrity value.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Signal windows of size 3 are:
    •   [1, 2, 3] → Checksum (XOR) = 0
    •   [2, 3, 4] → Checksum (XOR) = 5
    •   [3, 4, 5] → Checksum (XOR) = 2

Final Integrity Value = 0 ^ 5 ^ 2 = 7

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

Final Integrity Value = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (signal length) and K (window size).
- The second line contains N space-separated integers — the signal values.

## Output Format

- Return a single integer — the final integrity value.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, bit manipulation