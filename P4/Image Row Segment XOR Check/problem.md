## Title

Image Row Segment XOR Check

## Slug

image-row-segment-xor-check

## Difficulty

Easy

## Description

An image processing algorithm analyzes pixel data row by row. One row is represented as a sequence of pixel intensity values A₁, A₂, ..., Aₙ. To detect texture patterns, the algorithm examines segments (windows) of size K along the row. For each segment, it computes a value by XORing the pixel intensities within it. To get a summary value for the row's texture, all these segment values are XORed together. Calculate this final row summary value.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Pixel row windows of size 3:
    •   [1, 2, 3] → Segment Value (XOR) = 0
    •   [2, 3, 4] → Segment Value (XOR) = 5
    •   [3, 4, 5] → Segment Value (XOR) = 2

Final Row Summary = 0 ^ 5 ^ 2 = 7

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

Final Row Summary = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (row length) and K (window size).
- The second line contains N space-separated integers — the pixel intensity values.

## Output Format

- Return a single integer — the final row summary value.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9 (Assuming integer intensities)

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, image processing, bit manipulation