## Title

Starlight Intensity XOR Pattern

## Slug

starlight-intensity-xor-pattern

## Difficulty

Easy

## Description

An astronomer analyzes a sequence of light intensity measurements A₁, A₂, ..., Aₙ from a distant star. To detect periodic fluctuations, they examine the data within a sliding window of size K. For each window, a pattern value is calculated by XORing all intensity measurements inside it. To derive a single characteristic value for the entire observation period, all these pattern values are XORed together. Calculate this final characteristic value.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Intensity windows of size 3:
    •   [1, 2, 3] → Pattern Value (XOR) = 0
    •   [2, 3, 4] → Pattern Value (XOR) = 5
    •   [3, 4, 5] → Pattern Value (XOR) = 2

Final Characteristic Value = 0 ^ 5 ^ 2 = 7

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

Final Characteristic Value = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (number of measurements) and K (window size).
- The second line contains N space-separated integers — the intensity measurements.

## Output Format

- Return a single integer — the final characteristic value.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, astronomy, bit manipulation