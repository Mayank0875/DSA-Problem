## Title
Reading Challenge

## Slug
reading-challenge

## Difficulty
Medium

## Description
A student reads daily. 1 is Read, 0 is Skipped. They can use k 'catch-up' days to fill in gaps.

You track reading habits represented by an array `nums` consisting of 1s (reading days) and 0s (skipped days), and an integer `k`. You are allowed to catch up on at most `k` skipped dayss from the sequence.

Your task is to find the length of the longest contiguous sequence of reading dayss after performing the catch-ups. If the sequence contains no reading dayss even after optimal catch-ups, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After catching up on the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of reading dayss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can catch up on the skipped days at index 4 and the skipped days at index 7. The resulting segments of reading dayss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for reading days, 0 for skipped days).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of reading dayss.

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
