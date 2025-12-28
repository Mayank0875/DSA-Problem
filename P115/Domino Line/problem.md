## Title
Domino Line

## Slug
domino-line

## Difficulty
Medium

## Description
Dominoes are set up by size. A prankster swapped a middle section with random sizes.

A valid domino line must be sequential, meaning the sizes should appear in non-decreasing order.

However, a prank has inserted a chunk of incorrect sizes into the middle of the domino line, corrupting it. To fix this, you must remove a single contiguous sequence of sizes (a subarray) so that the remaining sizes form a sorted, non-decreasing sequence.

Your goal is to minimize the dominoes removed. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining sizes.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining domino line is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the domino line is strictly decreasing, we can only keep one size. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of sizes.
- The second line contains `n` space-separated integers representing the `sizes` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ sizes[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
