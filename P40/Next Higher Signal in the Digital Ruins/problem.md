## Title

Next Higher Signal in the Digital Ruins

## Slug

next-higher-signal-digital-ruins

## Difficulty

Easy

## Description

Explorers are scanning a series of ancient digital ruins, recording the strength of each signal they encounter. For every recorded signal, they need to determine the strength of the nearest future signal that is strictly stronger. This helps them map the progression of energy patterns within the ruins or pinpoint particularly potent sources. If no future signal is stronger (either because it is the last reading or all subsequent signals are weaker or equal), this should be noted. Can you compute this for each signal reading?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Signal 0 (500): Next higher is 600 (Signal 2). Output 600.
Signal 1 (400): Next higher is 600 (Signal 2). Output 600.
Signal 2 (600): Next higher is 700 (Signal 4). Output 700.
Signal 3 (300): Next higher is 700 (Signal 4). Output 700.
Signal 4 (700): Next higher is 800 (Signal 6). Output 800.
Signal 5 (450): Next higher is 800 (Signal 6). Output 800.
Signal 6 (800): No future signal is higher. Output -1.
Signal 7 (500): No future signal exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All signals are equal, so no future signal is stronger.

## Input Format

The first line contains a single integer n, the number of signals.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the recorded signal strengths.

## Output Format

Return array of integers. The i-th integer should be the strength of the nearest signal j > i such that a_j > a_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array