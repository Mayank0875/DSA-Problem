## Title
Diamond Clarity

## Slug
diamond-clarity

## Difficulty
Medium

## Description
Diamonds are sorted by clarity on a belt. A handful of unsorted gems fell onto the belt.

A valid conveyor belt must be sorted, meaning the clarity grades should appear in non-decreasing order.

However, an accident has inserted a chunk of incorrect clarity grades into the middle of the conveyor belt, corrupting it. To fix this, you must remove a single contiguous sequence of clarity grades (a subarray) so that the remaining clarity grades form a sorted, non-decreasing sequence.

Your goal is to minimize the gems removed. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining clarity grades.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining conveyor belt is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the conveyor belt is strictly decreasing, we can only keep one clarity grade. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of clarity grades.
- The second line contains `n` space-separated integers representing the `grades` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ grades[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
