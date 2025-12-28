## Title
Chemical pH Level

## Slug
chemical-ph-level

## Difficulty
Medium

## Description
Adding base to acid increases pH. An improperly mixed solution caused erratic pH readings.

A valid titration log must be neutralizing, meaning the pH levels should appear in non-decreasing order.

However, poor mixing has inserted a chunk of incorrect pH levels into the middle of the titration log, corrupting it. To fix this, you must remove a single contiguous sequence of pH levels (a subarray) so that the remaining pH levels form a sorted, non-decreasing sequence.

Your goal is to minimize the readings scrubbed. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining pH levels.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining titration log is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the titration log is strictly decreasing, we can only keep one pH level. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of pH levels.
- The second line contains `n` space-separated integers representing the `levels` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ levels[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
