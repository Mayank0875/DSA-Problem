## Title
Video Frame Timestamps

## Slug
video-frame-timestamps

## Difficulty
Medium

## Description
A video stream should have frames with increasing timestamps. A network lag caused a packet burst to arrive with mixed-up times.

A valid video buffer must be playable, meaning the timestamps should appear in non-decreasing order.

However, packet loss has inserted a chunk of incorrect timestamps into the middle of the video buffer, corrupting it. To fix this, you must remove a single contiguous sequence of timestamps (a subarray) so that the remaining timestamps form a sorted, non-decreasing sequence.

Your goal is to minimize the dropped frames. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining timestamps.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining video buffer is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the video buffer is strictly decreasing, we can only keep one timestamp. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of timestamps.
- The second line contains `n` space-separated integers representing the `timestamps` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ timestamps[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
