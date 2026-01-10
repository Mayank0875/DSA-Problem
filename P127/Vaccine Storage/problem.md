## Title
Vaccine Storage

## Slug
vaccine-storage

## Difficulty
Medium

## Description
A fridge logs temperature. 1 is Safe Range, 0 is Unsafe. Backup power can correct k unsafe intervals.

You monitor temperature logs represented by an array `nums` consisting of 1s (safe intervals) and 0s (unsafe intervals), and an integer `k`. You are allowed to correct at most `k` unsafe intervalss from the sequence.

Your task is to find the length of the longest contiguous sequence of safe intervalss after performing the corrections. If the sequence contains no safe intervalss even after optimal corrections, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After correcting the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of safe intervalss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can correct the unsafe intervals at index 4 and the unsafe intervals at index 7. The resulting segments of safe intervalss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for safe intervals, 0 for unsafe intervals).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of safe intervalss.

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
