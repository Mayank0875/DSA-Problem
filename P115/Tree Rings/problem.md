## Title
Tree Rings

## Slug
tree-rings

## Difficulty
Medium

## Description
Tree rings should grow wider in good years. A disease caused erratic growth patterns for a decade.

A valid ring pattern must be healthy, meaning the ring widths should appear in non-decreasing order.

However, a disease has inserted a chunk of incorrect ring widths into the middle of the ring pattern, corrupting it. To fix this, you must remove a single contiguous sequence of ring widths (a subarray) so that the remaining ring widths form a sorted, non-decreasing sequence.

Your goal is to minimize the years analyzed. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining ring widths.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining ring pattern is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the ring pattern is strictly decreasing, we can only keep one ring width. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of ring widths.
- The second line contains `n` space-separated integers representing the `widths` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ widths[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
