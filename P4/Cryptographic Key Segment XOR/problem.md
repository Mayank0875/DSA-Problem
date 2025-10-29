## Title

Cryptographic Key Segment XOR

## Slug

crypto-key-segment-xor

## Difficulty

Easy

## Description

A cryptographer is analyzing a long numerical key represented by an array A₁, A₂, ..., Aₙ. To find potential patterns, they examine contiguous segments (windows) of the key, each of size K. For every segment, they compute a segment hash by XORing all the numbers within it. To obtain a final combined hash representing the key's structure across all segments, they XOR all the computed segment hashes together. Your task is to calculate this final combined hash.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Key segments of size 3:
    •   [1, 2, 3] → Segment Hash (XOR) = 0
    •   [2, 3, 4] → Segment Hash (XOR) = 5
    •   [3, 4, 5] → Segment Hash (XOR) = 2

Final Combined Hash = 0 ^ 5 ^ 2 = 7

### 2

#### Input

4 2
[5, 1, 3, 2]

#### Output

7

#### Explanation

Segments:
    •   [5, 1] → XOR = 4
    •   [1, 3] → XOR = 2
    •   [3, 2] → XOR = 1

Final Combined Hash = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (key length) and K (segment size).
- The second line contains N space-separated integers — the key elements.

## Output Format

- Return a single integer — the final combined hash.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, cryptography, bit manipulation