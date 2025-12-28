## Title
Assembly Line Heights

## Slug
assembly-line-heights

## Difficulty
Medium

## Description
Robots on a line are arranged by height for efficiency. A maintenance crew mixed up a section of the robots.

A valid robot line must be ergonomic, meaning the heights should appear in non-decreasing order.

However, a scheduling mix-up has inserted a chunk of incorrect heights into the middle of the robot line, corrupting it. To fix this, you must remove a single contiguous sequence of heights (a subarray) so that the remaining heights form a sorted, non-decreasing sequence.

Your goal is to minimize the downtime. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining heights.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining robot line is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the robot line is strictly decreasing, we can only keep one height. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of heights.
- The second line contains `n` space-separated integers representing the `heights` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ heights[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
