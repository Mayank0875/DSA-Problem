## Title
Queue Wait Times

## Slug
queue-wait-times

## Difficulty
Medium

## Description
As a queue gets longer, wait times increase. A glitch in the estimation algorithm output random times.

A valid display board must be accurate, meaning the times should appear in non-decreasing order.

However, an algorithm glitch has inserted a chunk of incorrect times into the middle of the display board, corrupting it. To fix this, you must remove a single contiguous sequence of times (a subarray) so that the remaining times form a sorted, non-decreasing sequence.

Your goal is to minimize the estimates hidden. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining times.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining display board is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the display board is strictly decreasing, we can only keep one time. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of times.
- The second line contains `n` space-separated integers representing the `times` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ times[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
