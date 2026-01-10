## Title
Memory Recall

## Slug
memory-recall

## Difficulty
Medium

## Description
A subject recalls a list. 1 is Remembered, 0 is Forgotten. Hints can be given for k forgotten items.

You test memory recall represented by an array `nums` consisting of 1s (remembered items) and 0s (forgotten items), and an integer `k`. You are allowed to hint at most `k` forgotten itemss from the sequence.

Your task is to find the length of the longest contiguous sequence of remembered itemss after performing the hints. If the sequence contains no remembered itemss even after optimal hints, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After hinting the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of remembered itemss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can hint the forgotten items at index 4 and the forgotten items at index 7. The resulting segments of remembered itemss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for remembered items, 0 for forgotten items).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of remembered itemss.

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
