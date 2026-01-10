## Title
Exam Streak

## Slug
exam-streak

## Difficulty
Medium

## Description
A student takes a series of exams. Scores are marked as Pass (1) or Fail (0). The teacher allows retaking up to k failed exams to fix the grade record.

You have a record of exam results represented by an array `nums` consisting of 1s (passing grades) and 0s (failing grades), and an integer `k`. You are allowed to retake at most `k` failing gradess from the sequence.

Your task is to find the length of the longest contiguous sequence of passing gradess after performing the retakes. If the sequence contains no passing gradess even after optimal retakes, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After retaking the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of passing gradess has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can retake the failing grades at index 4 and the failing grades at index 7. The resulting segments of passing gradess merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for passing grades, 0 for failing grades).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of passing gradess.

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
