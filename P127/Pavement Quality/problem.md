## Title
Pavement Quality

## Slug
pavement-quality

## Difficulty
Medium

## Description
A road inspector checks segments. 1 is Smooth, 0 is Pothole. The crew can patch k potholes.

You inspect a road represented by an array `nums` consisting of 1s (smooth segments) and 0s (potholes), and an integer `k`. You are allowed to patch at most `k` potholess from the sequence.

Your task is to find the length of the longest contiguous sequence of smooth segmentss after performing the patches. If the sequence contains no smooth segmentss even after optimal patches, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After patching the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of smooth segmentss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can patch the potholes at index 4 and the potholes at index 7. The resulting segments of smooth segmentss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for smooth segments, 0 for potholes).
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
