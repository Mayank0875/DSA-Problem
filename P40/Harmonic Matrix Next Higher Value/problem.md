## Title

Harmonic Matrix Next Higher Value

## Slug

harmonic-matrix-next-higher-value

## Difficulty

Easy

## Description

A researcher is studying a harmonic matrix, which contains the amplitudes of different frequencies recorded over time. For each entry in the matrix (considered as a one‑dimensional sequence), they need to determine the amplitude of the nearest future entry that has a strictly higher value. This information helps in analyzing how the harmonic content evolves. If there is no later entry with a higher amplitude (either because it is the last entry or all subsequent entries are lower or equal), it should be indicated. Can you compute this for every position?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Concert 0 (500): Next higher is 600 (Concert 2). Output 600.
Concert 1 (400): Next higher is 600 (Concert 2). Output 600.
Concert 2 (600): Next higher is 700 (Concert 4). Output 700.
Concert 3 (300): Next higher is 700 (Concert 4). Output 700.
Concert 4 (700): Next higher is 800 (Concert 6). Output 800.
Concert 5 (450): Next higher is 800 (Concert 6). Output 800.
Concert 6 (800): No future concert is higher. Output -1.
Concert 7 (500): No future concert exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All Attendance are equal, so no future concert has higher attendance.

## Input Format

The first line contains a single integer n, the number of concerts.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the audience attendance for each concert.

## Output Format

Return array of integers. The i-th integer should be the attendance of the nearest concert j > i such that a_j > a_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array