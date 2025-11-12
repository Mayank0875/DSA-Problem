## Title

Lost Signal: Next Stronger Transmission

## Slug

lost-signal-next-stronger-transmission

## Difficulty

Easy

## Description

A communication team is analyzing the strength of received signals over time to anticipate future improvements. For each recorded signal, they want to identify the strength of the nearest later signal that is strictly stronger. This helps them understand signal quality trends or pinpoint moments of significant boost. If no later signal is stronger (either because it is the last record or all subsequent signals are weaker or equal), this should be noted. Can you calculate this for each signal?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Signal 0 (500): Next stronger is 600 (Signal 2). Output 600.
Signal 1 (400): Next stronger is 600 (Signal 2). Output 600.
Signal 2 (600): Next stronger is 700 (Signal 4). Output 700.
Signal 3 (300): Next stronger is 700 (Signal 4). Output 700.
Signal 4 (700): Next stronger is 800 (Signal 6). Output 800.
Signal 5 (450): Next stronger is 800 (Signal 6). Output 800.
Signal 6 (800): No later signal is stronger. Output -1.
Signal 7 (500): No later signal exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All signal strengths are equal, so no later signal is stronger.

## Input Format

The first line contains a single integer n, the number of signals.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the strength of each signal.

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