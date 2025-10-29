## Title

Packet Sequence XOR Checksum

## Slug

packet-sequence-xor-checksum

## Difficulty

Easy

## Description

A network administrator is analyzing a sequence of packet identifiers A₁, A₂, ..., Aₙ captured during a transmission. They suspect an anomaly might be detectable by examining checksums over consecutive subsequences (windows) of size K. For each window, a checksum is computed by XORing the identifiers within it. To get a single value summarizing the checksum behavior across the sequence, all window checksums are XORed together. Determine this final summary checksum.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Packet ID windows of size 3:
    •   [1, 2, 3] → Checksum (XOR) = 0
    •   [2, 3, 4] → Checksum (XOR) = 5
    •   [3, 4, 5] → Checksum (XOR) = 2

Final Summary Checksum = 0 ^ 5 ^ 2 = 7

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

Final Summary Checksum = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (number of packets) and K (window size).
- The second line contains N space-separated integers — the packet identifiers.

## Output Format

- Return a single integer — the final summary checksum.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, networking, bit manipulation