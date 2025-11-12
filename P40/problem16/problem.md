## Title

Next Higher Flow in a Parallel Stream

## Slug

next-higher-flow-parallel-stream

## Difficulty

Easy

## Description

A hydrologist is studying the flow rates of a series of parallel streams to predict future water availability. For each stream segment, they want to identify the flow rate of the nearest downstream segment that has a strictly higher flow. This helps in understanding how water volume changes along the network or spotting segments with unusually high discharge. If no downstream segment has a higher flow (either because it is the last segment or all subsequent segments have lower or equal flow), this should be noted. Can you calculate this for each segment?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Segment 0 (500): Next higher is 600 (Segment 2). Output 600.
Segment 1 (400): Next higher is 600 (Segment 2). Output 600.
Segment 2 (600): Next higher is 700 (Segment 4). Output 700.
Segment 3 (300): Next higher is 700 (Segment 4). Output 700.
Segment 4 (700): Next higher is 800 (Segment 6). Output 800.
Segment 5 (450): Next higher is 800 (Segment 6). Output 800.
Segment 6 (800): No downstream segment is higher. Output -1.
Segment 7 (500): No downstream segment exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All flow rates are equal, so no downstream segment has higher flow.

## Input Format

The first line contains a single integer n, the number of stream segments.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the flow rate for each segment.

## Output Format

Return array of integers. The i-th integer should be the flow rate of the nearest segment j > i such that a_j > a_i. If no such segment exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array