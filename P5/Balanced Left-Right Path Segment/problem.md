## Title

Balanced Left-Right Path Segment

## Slug

balanced-lr-path-segment

## Difficulty

Easy

## Description

Consider a path traced within a binary search tree, where each step is recorded as '0' for moving to a left child and '1' for moving to a right child. We want to find the longest contiguous sub-path within this trace where the number of left moves equals the number of right moves. This signifies a balanced exploration segment. Given the sequence of moves, determine the length of the longest balanced sub-path.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The path segment [0, 1] (Left, Right) is the longest balanced segment.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] (Left, Right) and [1, 0] (Right, Left) are the longest balanced segments.

## Input Format

- The first line contains a single integer N, the total number of moves in the path trace.
- The second line contains N space-separated integers, representing the moves (0 for left, 1 for right).

## Output Format

- Return a single integer representing the length of the longest contiguous balanced sub-path.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, trees, prefix sum, hashmap