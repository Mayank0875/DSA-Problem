## Title

Balanced Quality Check Segment

## Slug

balanced-quality-check-segment

## Difficulty

Easy

## Description

An assembly line has N checkpoints. At each checkpoint, a product either passes ('1') or fails ('0') inspection. We need to find the longest continuous segment of checkpoints where the number of passed inspections equals the number of failed inspections. This helps identify sections of the line with consistent but mixed quality results. Given the sequence of inspection outcomes, find the length of the longest balanced segment.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The segment [0, 1] (Fail, Pass) is the longest balanced segment.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] (Fail, Pass) and [1, 0] (Pass, Fail) are the longest balanced segments.

## Input Format

- The first line contains a single integer N, the number of checkpoints.
- The second line contains N space-separated integers, representing inspection outcomes (0 for fail, 1 for pass).

## Output Format

- Return a single integer representing the length of the longest contiguous balanced segment.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, manufacturing, prefix sum, hashmap