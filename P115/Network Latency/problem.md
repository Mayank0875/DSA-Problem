## Title
Network Latency

## Slug
network-latency

## Difficulty
Medium

## Description
As distance increases, latency should increase. Routing errors caused some distant nodes to report impossibly low latency.

A valid ping report must be logical, meaning the latencies should appear in non-decreasing order.

However, routing errors has inserted a chunk of incorrect latencies into the middle of the ping report, corrupting it. To fix this, you must remove a single contiguous sequence of latencies (a subarray) so that the remaining latencies form a sorted, non-decreasing sequence.

Your goal is to minimize the nodes re-tested. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining latencies.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining ping report is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the ping report is strictly decreasing, we can only keep one latency. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of latencies.
- The second line contains `n` space-separated integers representing the `latencies` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ latencies[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
