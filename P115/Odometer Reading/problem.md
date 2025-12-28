## Title
Odometer Reading

## Slug
odometer-reading

## Difficulty
Medium

## Description
Mileage always increases. Tampering caused the odometer to show lower numbers intermittently.

A valid mileage log must be increasing, meaning the miles should appear in non-decreasing order.

However, tampering has inserted a chunk of incorrect miles into the middle of the mileage log, corrupting it. To fix this, you must remove a single contiguous sequence of miles (a subarray) so that the remaining miles form a sorted, non-decreasing sequence.

Your goal is to minimize the logs invalidated. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining miles.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining mileage log is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the mileage log is strictly decreasing, we can only keep one mile. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of miles.
- The second line contains `n` space-separated integers representing the `miles` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ miles[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
