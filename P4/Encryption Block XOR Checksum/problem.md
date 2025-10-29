## Title

Encryption Block XOR Checksum

## Slug

encryption-block-xor-checksum

## Difficulty

Easy

## Description

An encryption process generates a sequence of intermediate numerical blocks A₁, A₂, ..., Aₙ. To ensure integrity during the process, checksums are calculated over sliding windows of K blocks. For each window, the checksum is the XOR sum of the block values within it. A final master checksum is computed by XORing all the individual window checksums. Your task is to compute this master checksum for the given sequence of blocks.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Block windows of size 3:
    •   [1, 2, 3] → Window Checksum (XOR) = 0
    •   [2, 3, 4] → Window Checksum (XOR) = 5
    •   [3, 4, 5] → Window Checksum (XOR) = 2

Master Checksum = 0 ^ 5 ^ 2 = 7

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

Master Checksum = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (number of blocks) and K (window size).
- The second line contains N space-separated integers — the block values.

## Output Format

- Return a single integer — the final master checksum.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, encryption, bit manipulation