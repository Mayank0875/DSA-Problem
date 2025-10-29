## Title

Sensor Window XOR Aggregate

## Slug

sensor-window-xor-aggregate

## Difficulty

Easy

## Description

An environmental monitoring station records sensor readings A₁, A₂, ..., Aₙ over a period. To analyze short-term fluctuations, data scientists look at readings within a sliding window of size K. For each window, they calculate an aggregate value by XORing all readings in that window. To produce a single representative value for the entire monitoring period, reflecting these fluctuations, they XOR all the window aggregate values. Calculate this final representative value.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Sensor reading windows of size 3:
    •   [1, 2, 3] → Aggregate (XOR) = 0
    •   [2, 3, 4] → Aggregate (XOR) = 5
    •   [3, 4, 5] → Aggregate (XOR) = 2

Final Representative Value = 0 ^ 5 ^ 2 = 7

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

Final Representative Value = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (number of readings) and K (window size).
- The second line contains N space-separated integers — the sensor readings.

## Output Format

- Return a single integer — the final representative value.

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