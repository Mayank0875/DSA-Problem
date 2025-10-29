## Title

Balanced Robot Path

## Slug

balanced-robot-path

## Difficulty

Easy

## Description

A robot moves along a line, recording its movements as a sequence. A '0' represents a move to the left, and a '1' represents a move to the right. We need to analyze the robot's movement log. Your task is to find the length of the longest continuous segment of the robot's path where the number of left moves ('0') is exactly equal to the number of right moves ('1'), indicating a balanced segment of movement.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The path [0, 1] (Left, Right) is the longest segment with an equal number of left and right moves.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

Segments [0, 1] (Left, Right) and [1, 0] (Right, Left) are the longest balanced segments.

## Input Format

- The first line contains a single integer N, the total number of moves recorded.
- The second line contains N space-separated integers, where each integer is either 0 (Left) or 1 (Right).

## Output Format

- Return a single integer representing the length of the longest contiguous segment with an equal number of 0s and 1s.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hashmap