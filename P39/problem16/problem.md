## Title

Parallel Stream Flow

## Slug

parallel-stream-flow

## Difficulty

Easy

## Description

Imagine observing a sequence of parallel streams, each with its own flow rate. As you stand at a particular stream, you look upstream (to your left) and want to know the flow rate of the nearest stream that is strictly higher than the one you are currently observing. If all upstream streams have lower or equal flow, or if it's the first stream, there is no such higher‑flow stream to the left. Your goal is to determine this higher flow rate for each position in the sequence.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Stream 0 (30): No previous stream. Output -1.
Stream 1 (60): Stream 0 (30) is lower. Output -1.
Stream 2 (90): Streams 0 (30), 1 (60) are lower. Output -1.
Stream 3 (50): Stream 2 (90) is the nearest higher. Output 90.
Stream 4 (80): Stream 2 (90) is the nearest higher. Output 90.
Stream 5 (40): Stream 4 (80) is the nearest higher. Output 80.
Stream 6 (70): Stream 4 (80) is the nearest higher. Output 80.
Stream 7 (50): Stream 6 (70) is the nearest higher. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All streams have equal flow, so no strictly higher upstream stream exists.

## Input Format

The first line contains a single integer n, the number of streams.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the flow rate of each stream.

## Output Format

Return array of integers. The i-th integer should be the flow rate of the nearest stream j < i such that h_j > h_i. If no such stream exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array