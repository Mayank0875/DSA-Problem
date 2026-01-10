## Title
Archery Practice

## Slug
archery-practice

## Difficulty
Medium

## Description
An archer shoots arrows. 1 is Bullseye, 0 is Outer Ring. They can claim k outer ring shots were 'practice' and ignore them.

You score archery shots represented by an array `nums` consisting of 1s (bullseyes) and 0s (outer ring shots), and an integer `k`. You are allowed to ignore at most `k` outer ring shotss from the sequence.

Your task is to find the length of the longest contiguous sequence of bullseyess after performing the discards. If the sequence contains no bullseyess even after optimal discards, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After ignoring the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of bullseyess has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can ignore the outer ring shots at index 4 and the outer ring shots at index 7. The resulting segments of bullseyess merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for bullseyes, 0 for outer ring shots).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of bullseyess.

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
