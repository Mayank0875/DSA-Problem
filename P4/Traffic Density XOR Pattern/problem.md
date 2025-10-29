## Title

Traffic Density XOR Pattern

## Slug

traffic-density-xor-pattern

## Difficulty

Easy

## Description

A traffic monitoring system records the number of vehicles passing a point at different time intervals, resulting in a sequence A₁, A₂, ..., Aₙ. To analyze congestion patterns over K intervals, analysts use a sliding window. For each window, they calculate a pattern value by XORing the vehicle counts within it. To obtain a single value summarizing the flow pattern for the entire observation period, they XOR all the calculated window pattern values. Compute this final traffic pattern value.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Vehicle count windows of size 3:
    •   [1, 2, 3] → Pattern Value (XOR) = 0
    •   [2, 3, 4] → Pattern Value (XOR) = 5
    •   [3, 4, 5] → Pattern Value (XOR) = 2

Final Traffic Pattern Value = 0 ^ 5 ^ 2 = 7

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

Final Traffic Pattern Value = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (number of intervals) and K (window size).
- The second line contains N space-separated integers — the vehicle counts.

## Output Format

- Return a single integer — the final traffic pattern value.

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