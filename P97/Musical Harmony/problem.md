## Title
Musical Harmony

## Slug
musical-harmony

## Difficulty
Hard

## Description
A composer arranges notes. A melody is 'harmonically pure' if the sum of the note frequencies matches the lowest missing frequency in the scale.

Maestro is analyzing a sequence of n notes. Each note has a specific frequency index (a non-negative integer).

A contiguous group of notes is considered **pure** if the sum of their frequency index values is exactly equal to the **Silent Note** of that group.

The Silent Note (Minimum Excluded Value or MEX) is defined as the smallest non-negative integer that does not exist among the frequency index values in the group.
For example:
- MEX of [1, 2] is 0
- MEX of [0, 2] is 1
- MEX of [0, 1, 2] is 3

Your task is to count the number of non-empty continuous subsegments that are pure.

## Examples

### 1

#### Input
5
0 1 2 0 1

#### Output
4

#### Explanation
The pure subsegments are:
- `[0, 1, 2]` (Indices 0-2): Sum = 3, MEX = 3.
- `[1, 2, 0]` (Indices 1-3): Sum = 3, MEX = 3.
- `[2, 0, 1]` (Indices 2-4): Sum = 3, MEX = 3.
- `[0, 1, 2, 0]` (Indices 0-3): Sum = 3, MEX = 3.

### 2

#### Input
3
1 1 1

#### Output
0

#### Explanation
No subsegment satisfies the condition. For `[1]`, Sum=1, MEX=0.

## Input Format
- The first line contains a single integer $n$ — the number of notes.
- The second line contains $n$ space-separated integers representing the frequency index values.

## Output Format
- Return a single integer representing the number of pure subsegments.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ frequency index ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, maths, array
