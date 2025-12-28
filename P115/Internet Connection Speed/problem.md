## Title
Internet Connection Speed

## Slug
internet-connection-speed

## Difficulty
Medium

## Description
A speed test ramps up bandwidth usage. Congestion caused the speed to fluctuate wildly.

A valid speed test must be stable, meaning the Mbps should appear in non-decreasing order.

However, congestion has inserted a chunk of incorrect Mbps into the middle of the speed test, corrupting it. To fix this, you must remove a single contiguous sequence of Mbps (a subarray) so that the remaining Mbps form a sorted, non-decreasing sequence.

Your goal is to minimize the test phase skipped. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining Mbps.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining speed test is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the speed test is strictly decreasing, we can only keep one Mbp. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of Mbps.
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
