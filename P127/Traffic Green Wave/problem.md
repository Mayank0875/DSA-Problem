## Title
Traffic Green Wave

## Slug
traffic-green-wave

## Difficulty
Medium

## Description
A driver hits a series of traffic lights. 1 is Green, 0 is Red. The car has a smart system that can legally bypass up to k red lights using express lanes.

You encounter a sequence of traffic lights represented by an array `nums` consisting of 1s (green lights) and 0s (red lights), and an integer `k`. You are allowed to bypass at most `k` red lightss from the sequence.

Your task is to find the length of the longest contiguous sequence of green lightss after performing the bypasses. If the sequence contains no green lightss even after optimal bypasses, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After bypassing the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of green lightss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can bypass the red lights at index 4 and the red lights at index 7. The resulting segments of green lightss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for green lights, 0 for red lights).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of green lightss.

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
