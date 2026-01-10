## Title
Music Rhythm

## Slug
music-rhythm

## Difficulty
Medium

## Description
A drummer hits beats. 1 is On-Beat, 0 is Off-Beat. A quantization tool can align up to k off-beats.

You analyze a drum track represented by an array `nums` consisting of 1s (perfect beats) and 0s (mistakes), and an integer `k`. You are allowed to align at most `k` mistakess from the sequence.

Your task is to find the length of the longest contiguous sequence of perfect beatss after performing the alignments. If the sequence contains no perfect beatss even after optimal alignments, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After aligning the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of perfect beatss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can align the mistakes at index 4 and the mistakes at index 7. The resulting segments of perfect beatss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for perfect beats, 0 for mistakes).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of perfect beatss.

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
