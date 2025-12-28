## Title
Marathon Pace

## Slug
marathon-pace

## Difficulty
Medium

## Description
A runner tries to negatively split (get faster or steady). A cramp caused a section of slow/erratic splits in the middle.

A valid split log must be negative split, meaning the split times should appear in non-increasing order.

However, a cramp has inserted a chunk of incorrect split times into the middle of the split log, corrupting it. To fix this, you must remove a single contiguous sequence of split times (a subarray) so that the remaining split times form a sorted, non-increasing sequence.

Your goal is to minimize the data excluded. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-increasing order of the remaining split times.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining split log is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the split log is strictly decreasing, we can only keep one split time. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of split times.
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
