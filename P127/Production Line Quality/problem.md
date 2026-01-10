## Title
Production Line Quality

## Slug
production-line-quality

## Difficulty
Medium

## Description
A factory belt has items. 1 is Good, 0 is Defective. A robot arm can remove up to k defective items to create a continuous run of good products.

You inspect a production line represented by an array `nums` consisting of 1s (good items) and 0s (defective items), and an integer `k`. You are allowed to remove at most `k` defective itemss from the sequence.

Your task is to find the length of the longest contiguous sequence of good itemss after performing the removals. If the sequence contains no good itemss even after optimal removals, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After removing the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of good itemss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can remove the defective items at index 4 and the defective items at index 7. The resulting segments of good itemss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for good items, 0 for defective items).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of good itemss.

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
