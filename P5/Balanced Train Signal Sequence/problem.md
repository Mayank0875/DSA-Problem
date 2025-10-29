## Title

Balanced Train Signal Sequence

## Slug

balanced-train-signal-sequence

## Difficulty

Easy

## Description

A train control system logs signal states along a track section as a sequence of 0s and 1s, representing two possible signal aspects (e.g., clear/stop). For safety analysis, find the longest contiguous sequence of signals where the count of '0' aspects equals the count of '1' aspects. This might represent a specific signaling block or a balanced operational phase. Determine the length of the longest such balanced signal sequence.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The sequence [0, 1] is the longest balanced signal sequence.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] and [1, 0] are the longest balanced signal sequences.

## Input Format

- The first line contains a single integer N, the length of the signal log.
- The second line contains N space-separated integers, representing the signal states (0 or 1).

## Output Format

- Return a single integer representing the length of the longest contiguous balanced signal sequence.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hashmap