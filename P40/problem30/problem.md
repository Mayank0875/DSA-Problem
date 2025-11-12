## Title

Next Higher Signal in Digital Ruins

## Slug

next-higher-signal-digital-ruins

## Difficulty

Easy

## Description

Explorers are scanning the remnants of an ancient digital archive, known as the Digital Ruins. For each data pulse recorded, they need to determine the value of the nearest future pulse that exhibits a strictly higher signal strength. This information helps them map the growth patterns of the lost civilization’s data streams or pinpoint particularly powerful transmissions. If no future pulse has a higher strength (either because it is the last pulse or all subsequent pulses are weaker or equal), this should be indicated. Can you compute this for each pulse?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Pulse 0 (500): Next higher is 600 (Pulse 2). Output 600.
Pulse 1 (400): Next higher is 600 (Pulse 2). Output 600.
Pulse 2 (600): Next higher is 700 (Pulse 4). Output 700.
Pulse 3 (300): Next higher is 700 (Pulse 4). Output 700.
Pulse 4 (700): Next higher is 800 (Pulse 6). Output 800.
Pulse 5 (450): Next higher is 800 (Pulse 6). Output 800.
Pulse 6 (800): No future pulse is higher. Output -1.
Pulse 7 (500): No future pulse exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All signal strengths are equal, so no future pulse has a higher strength.

## Input Format

The first line contains a single integer n, the number of pulses.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the signal strength for each pulse.

## Output Format

Return array of integers. The i-th integer should be the strength of the nearest pulse j > i such that a_j > a_i. If no such pulse exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array