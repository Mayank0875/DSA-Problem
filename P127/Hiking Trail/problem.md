## Title
Hiking Trail

## Slug
hiking-trail

## Difficulty
Medium

## Description
A trail has segments. 1 is Clear, 0 is Blocked. A park ranger can clear k blocked segments to open a path.

You map a hiking trail represented by an array `nums` consisting of 1s (clear paths) and 0s (blocked paths), and an integer `k`. You are allowed to clear at most `k` blocked pathss from the sequence.

Your task is to find the length of the longest contiguous sequence of clear pathss after performing the clearances. If the sequence contains no clear pathss even after optimal clearances, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After clearing the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of clear pathss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can clear the blocked paths at index 4 and the blocked paths at index 7. The resulting segments of clear pathss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for clear paths, 0 for blocked paths).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of clear pathss.

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
