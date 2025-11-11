## Title

Bitstream Echo

## Slug

bitstream-echo

## Difficulty

Medium

## Description

In a high‑speed data center, engineers are arranging identical data packets on a two‑dimensional memory grid before transmission.  
Each packet occupies a rectangle of width **w** bits and height **h** bits. All packets must be placed flat (no rotation) inside a single square memory buffer.  
Given **n** such packets, determine the smallest possible side length of the square buffer that can contain all packets without overlap.

## Examples

### 1

#### Input

2 3 10

#### Output

9

#### Explanation

A square of side 9 fits floor(9/2) = 4 packets across and floor(9/3) = 3 packets down, giving 4 × 3 = 12 packets — enough for 10.  
A square of side 8 fits floor(8/2) × floor(8/3) = 4 × 2 = 8 packets — not enough.  
Hence, the minimum side length is 9.

### 2

#### Input

1 1 3

#### Output

2

#### Explanation

A square of side 2 fits floor(2/1) × floor(2/1) = 2 × 2 = 4 packets.  
A square of side 1 fits only 1 × 1 = 1 packet.  
Therefore, the minimum side length needed for 3 packets is 2.
  
## Input Format  

- Three space-separated integers w, h, and n.

## Output Format  

- Return single integer representing the minimum side length of the square buffer.
  

## Constraints  

- 1 ≤ w, h, n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory