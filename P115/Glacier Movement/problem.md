## Title
Glacier Movement

## Slug
glacier-movement

## Difficulty
Medium

## Description
Glaciers move faster towards the center/end. A sensor error recorded random speeds in a specific zone.

A valid flow model must be accurate, meaning the speeds should appear in non-decreasing order.

However, sensor noise has inserted a chunk of incorrect speeds into the middle of the flow model, corrupting it. To fix this, you must remove a single contiguous sequence of speeds (a subarray) so that the remaining speeds form a sorted, non-decreasing sequence.

Your goal is to minimize the data points dropped. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining speeds.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining flow model is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the flow model is strictly decreasing, we can only keep one speed. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of speeds.
- The second line contains `n` space-separated integers representing the `speeds` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ speeds[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
