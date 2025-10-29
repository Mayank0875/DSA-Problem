## Title

Robot Path Sensor XOR Fusion

## Slug

robot-path-sensor-xor-fusion

## Difficulty

Easy

## Description

A robot moving along a path records sensor readings A₁, A₂, ..., Aₙ. To fuse sensor data over short path segments, the robot processes readings within a sliding window of size K. For each window, it calculates a fused value by XORing all sensor readings in that window. To generate a single value representing the fused data across the entire path, it XORs all the fused values from each window. Calculate this final fused value for the robot's path.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Sensor windows of size 3:
    •   [1, 2, 3] → Fused Value (XOR) = 0
    •   [2, 3, 4] → Fused Value (XOR) = 5
    •   [3, 4, 5] → Fused Value (XOR) = 2

Final Fused Value = 0 ^ 5 ^ 2 = 7

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

Final Fused Value = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (number of readings) and K (window size).
- The second line contains N space-separated integers — the sensor readings.

## Output Format

- Return a single integer — the final fused value.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, robotics, bit manipulation