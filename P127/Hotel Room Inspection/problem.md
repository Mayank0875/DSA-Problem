## Title
Hotel Room Inspection

## Slug
hotel-room-inspection

## Difficulty
Medium

## Description
A manager checks rooms. 1 is Clean, 0 is Dirty. Housekeeping can quick-clean k dirty rooms.

You inspect hotel rooms represented by an array `nums` consisting of 1s (clean rooms) and 0s (dirty rooms), and an integer `k`. You are allowed to clean at most `k` dirty roomss from the sequence.

Your task is to find the length of the longest contiguous sequence of clean roomss after performing the cleanings. If the sequence contains no clean roomss even after optimal cleanings, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After cleaning the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of clean roomss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can clean the dirty rooms at index 4 and the dirty rooms at index 7. The resulting segments of clean roomss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for clean rooms, 0 for dirty rooms).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of clean roomss.

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
