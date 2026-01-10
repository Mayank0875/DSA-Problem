## Title
Diet Adherence

## Slug
diet-adherence

## Difficulty
Medium

## Description
A person tracks their diet. 1 is Healthy, 0 is Cheat Meal. They allow themselves k 'cheat days' to be ignored in the streak count.

You track daily meals represented by an array `nums` consisting of 1s (healthy days) and 0s (cheat days), and an integer `k`. You are allowed to ignore at most `k` cheat dayss from the sequence.

Your task is to find the length of the longest contiguous sequence of healthy dayss after performing the passes. If the sequence contains no healthy dayss even after optimal passes, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After ignoring the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of healthy dayss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can ignore the cheat days at index 4 and the cheat days at index 7. The resulting segments of healthy dayss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for healthy days, 0 for cheat days).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of healthy dayss.

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
