## Title
Streaming Buffer

## Slug
streaming-buffer

## Difficulty
Medium

## Description
A video stream has segments. 1 is Smooth, 0 is Buffering. The player pre-loader can smooth over k buffering segments.

You monitor a video stream represented by an array `nums` consisting of 1s (smooth segments) and 0s (buffering segments), and an integer `k`. You are allowed to smooth at most `k` buffering segmentss from the sequence.

Your task is to find the length of the longest contiguous sequence of smooth segmentss after performing the fixes. If the sequence contains no smooth segmentss even after optimal fixes, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After smoothing the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of smooth segmentss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can smooth the buffering segments at index 4 and the buffering segments at index 7. The resulting segments of smooth segmentss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for smooth segments, 0 for buffering segments).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of smooth segmentss.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ nums[i] ≤ 1
- 0 ≤ k ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sliding-window, two-pointers, array

## Company
facebook
