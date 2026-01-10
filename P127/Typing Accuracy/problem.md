## Title
Typing Accuracy

## Slug
typing-accuracy

## Difficulty
Medium

## Description
A typist types a stream of characters. 1 is Correct, 0 is Typo. Autocorrect can fix up to k typos automatically.

You analyze keystrokes represented by an array `nums` consisting of 1s (correct keys) and 0s (typos), and an integer `k`. You are allowed to correct at most `k` typoss from the sequence.

Your task is to find the length of the longest contiguous sequence of correct keyss after performing the corrections. If the sequence contains no correct keyss even after optimal corrections, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After correcting the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of correct keyss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can correct the typos at index 4 and the typos at index 7. The resulting segments of correct keyss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for correct keys, 0 for typos).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of correct keyss.

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
