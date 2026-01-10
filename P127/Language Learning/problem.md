## Title
Language Learning

## Slug
language-learning

## Difficulty
Medium

## Description
A user practices daily. 1 is Practice, 0 is Missed. The app has k 'streak freeze' items to save the streak.

You track daily practice represented by an array `nums` consisting of 1s (practice days) and 0s (missed days), and an integer `k`. You are allowed to freeze at most `k` missed dayss from the sequence.

Your task is to find the length of the longest contiguous sequence of practice dayss after performing the freezes. If the sequence contains no practice dayss even after optimal freezes, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After freezing the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of practice dayss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can freeze the missed days at index 4 and the missed days at index 7. The resulting segments of practice dayss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for practice days, 0 for missed days).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of practice dayss.

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
