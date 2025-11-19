## Title

Previous Stronger Signal

## Slug

silent-transmission

## Difficulty

Easy

## Description

Imagine moving along a line of communication devices, each emitting a signal of a certain strength. As you stand at each device, you look back (to your left) and want to know the strength of the nearest device that is strictly stronger than the one you are currently at. If all previous devices are weaker or of equal strength, or if it's the first device, there is no such stronger device to the left. Your goal is to determine this stronger device's signal strength for each position along the line.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Device 0 (30): No previous device. Output -1.
Device 1 (60): Device 0 (30) is weaker. Output -1.
Device 2 (90): Devices 0 (30), 1 (60) are weaker. Output -1.
Device 3 (50): Device 2 (90) is the nearest stronger. Output 90.
Device 4 (80): Device 2 (90) is the nearest stronger. Output 90.
Device 5 (40): Device 4 (80) is the nearest stronger. Output 80.
Device 6 (70): Device 4 (80) is the nearest stronger. Output 80.
Device 7 (50): Device 6 (70) is the nearest stronger. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All devices have equal strength, so no strictly stronger previous device exists.

## Input Format

The first line contains a single integer n, the number of devices.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the signal strength of each device.

## Output Format

Return array of integers. The i-th integer should be the strength of the nearest device j < i such that h_j > h_i. If no such device exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array